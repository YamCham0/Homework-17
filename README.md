# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Email expression that is simple. Numbers and letters are permitted before the @, and top level domains with fewer than two or more than three letters are not permitted.
```
Matching an Email:  
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,63})$/`
```
## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
The $ anchor denotes a string that ends with the characters that come before it. It, like the (^)character, can be preceded by an exact string or a range of possible matches.
``` ^\  (used at the beginning of the line) ```  \\\
``` \$  (used at the beginning of the line)```
### Quantifiers
Quantifiers define the length of the string that your regex will match. They regularly include minimum and maximum number of characters that your regex expects.
```
{2,63} will match 2 to 63.
```
### Grouping Constructs
As regular expressions become more complex, you may want to check multiple parts of a string to see if different sections meet different requirements. You'll need to use grouping constructs to separate these sections.
Parentheses (()) are the most common way to group a section of a regex. Each section enclosed by parentheses is referred to as a subexpression.
```
 First group ([a-z0-9_\.-]+)  
Second group ([\da-z\.-]+)  
Third gorup ([a-z\.]{2,63})

```

### Bracket Expressions
Anything enclosed in square brackets [] represents a set of characters we want to match. These expressions can be written to include all of the characters we want to match. For example, [abc] will look for a string that contains a, b, or c, regardless of its length.

```
[a-z0-9_\.-] it will match lower case and numbers with some special characters.
```
### Character Classes
The letter d corresponds to any single character that is a digit. The entire expression is searching for a domain name.

```  
\da-z\  
```

### The OR Operator
It functions similarly to a boolean OR. The expression before or after the | is matched.
It can operate on a single expression or on a group of expressions. The patterns will be tested in the order listed.


### Flags
Flags are added to the end of a regex after the second slash to define additional functionality or limits for the regex. There are six optional flags to choose from, here some examples:

```
g—Global search: the regex should be tested against all possible string matches.

i—Case-insensitive search: When looking for a match in a string, case should be ignored.

m—Multi-line search: a multi-line input string should be interpreted as multiple lines.
```
### Character Escapes
In a regex, the backslash ( \ ) escapes a character that would otherwise be interpreted literally. For example, the open bracket ( [ ) is used to start a Bracket Expression, but adding a backslash before the open square bracket ( \ [ ) tells the regex to look for the open square bracket character rather than starting to define a Bracket Expression.
## Author

By: Yamil Chamochumbi  
[Link Here]: (https://github.com/YamCham0)
