## Regex-Project 
As a web development student I want a tutorial explaining a specific regular expression so that I can understand the search pattern the regex defines.

## Summary
Using the following regular expression can be used to verify a search for a email address. 

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

During this gist we will explain and break down each part of the expression describing what it does.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy Match](#greedy-match)

## Regex Components

### Anchors
At the start of the expression you can find the `^` anchor. This is the beginning of a string. At the end of the string you find `$` and this determines the end of the string. Both are not effected by the multiline flags since it is not utilized within this expression.

### Quantifiers
By using the `+` as a quantifier, this matches one or more of preceeding sets of classes found in square backets. In the first bracket expression `[a-z0-9_\.-]` the possibilities would include characters a-z (case sensitive), numbers 0-9, underscore, period or hyphen. In the second bracket set `[\da-z\.-]`, the expression uses the quantifer to match any digit 0-9, a-z (case sensitive), period, or hyphen. The last quantifer is used in the last grouping where `{2,6}` matches a specified of atleast 2 but no more than 6 characters from the preceeding bracket expression `[a-z\.]`.

### Character Classes
The classes that are used in the expression are a character set with a range for number digit or letter from a-z. There is an escape character class incorporated searching for a dot notation `\.`. This escaped character can be found in all three bracket expressions. Furthermore, the `\d` character class can found with second grouping. This matches any digit character. Lastly, right after the first grouping you can find a punctuation character `@` and this will ensure there is always an at symbol between the username section and domain section when verifying an email address. 

### Grouping and Capturing
Parenthesis used within this expression capture a grouping of a string and can be defined as the following `(....)`. This can be used for extracting a subtring or using a back reference if needed in future expressions.

### Bracket Expressions
Three bracket expressions `[...]` can be found within this within each grouping. Within each set of brackets various character classes can be found. 

### Greedy Match
By default, the quantifer that allows the greedy match The quantifer that triggers the greedy match is `+`. This match will reference preceding characters as many times as possible. Towards the end of the expression `{2,6}` also tries to use its default greedy match by trying to match a minimum of two of the characters, but no more than six.


## Author

Adam Castro</br>
Github: https://github.com/avc0021</br>
Email: avc0021@gmail.com
