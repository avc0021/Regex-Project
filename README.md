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
`^` is start of string and the `$` determines the end of the string. 

### Quantifiers
`+` matches one or more of preceeding token.

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

 
