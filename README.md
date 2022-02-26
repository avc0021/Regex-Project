## Regex-Project 
As a web development student I want a tutorial explaining a specific regular expression so that I can understand the search pattern the regex defines.

## Summary
Using the following expression will allow a user to search for a email address. 

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

During this gist we will explain and break down each part of the expression describing what it does.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy Match](#greedy-match)
- [Boundaries](#boundaries)

## Regex Components

### Anchors
The `^` anchor is the beginning of a string, while `$` determines the end of the string. Both are not effected by the multiline flag since it is not enabled.

### Quantifiers
Using `+` as a quantifier matches one or more of preceeding sets of characters. In the first set `[a-z0-9_\.-]` this would include characters a-z (case sensitive), numbers 0-9, underscore, period or hyphen. In the second character set `[\da-z\.-]`uses the quantifer to match any digit 0-9, a-z (case sensitive), period, or hyphen. The last quantifer is used in the last grouping where `{2,6}` matches a specified quantity between 2 to 6.

### Character Classes
`a-z` and `0-9`

### Grouping and Capturing
Grouping allows you to treat another expression as a single unit. Using `(....)` will allow the first grouping.

### Bracket Expressions
`[...]` is a character class allows a specific set of characters.
### Greedy Match
`+`	Match the preceding character or subexpression 1 or more times (as many as possible).

### Boundaries
At the start and end of the this expression you can the boundry points `/.../`


## Author

Github: https://github.com/avc0021</br>
Email: avc0021@gmail.com

 
