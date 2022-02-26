## Regex-Project 
As a web development student I want a tutorial explaining a specific regular expression so that I can understand the search pattern the regex defines.

## Summary
Using the following expression will allow a user to search for a email address. 

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

During this gist we will explain and break down each part of the expression describing what it does.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Class/Set](#character-class/set)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy Match](#greedy-match)
- [Boundaries](#boundaries)

## Regex Components

### Anchors
The `^` anchor is the beginning of a string, while `$` determines the end of the string. Both are not effected by the multiline flag since it is not enabled.

### Quantifiers
By using the `+` as a quantifier matches one or more of preceeding sets of characters. In the first set `[a-z0-9_\.-]` this would include characters a-z (case sensitive), numbers 0-9, underscore, period or hyphen. In the second character set `[\da-z\.-]`uses the quantifer to match any digit 0-9, a-z (case sensitive), period, or hyphen. The last quantifer is used in the last grouping where `{2,6}` matches a specified quantity between 2 to 6.

### Character Class/Set
Character classes, also known as sets, are recognized by the usage of the square brackets or `[..]`. By identifying this character set it allows quantifier to look for one or more within this character set. 

### Grouping and Capturing
Parenthesis used within this expression capture a grouping of a string `(....)`. In this expression three groupings can be found. Later this can be used for extracting a subtring or using a back reference if needed. 

### Bracket Expressions
`[...]` is a character class allows a specific set of characters.

### Greedy Match
`+`	Match the preceding character or subexpression 1 or more times (as many as possible).

### Boundaries
At the start and end of the this expression you can the boundry points `/.../`


## Author

Github: https://github.com/avc0021</br>
Email: avc0021@gmail.com

 
