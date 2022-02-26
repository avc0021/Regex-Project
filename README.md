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

## Regex Components

### Anchors
At the start of the expression you can find the `^` anchor. This is the beginning of a string. At the end of the string you find `$` determines the end of the string. Both are not effected by the multiline flags since it is not enabled.

### Quantifiers
By using the `+` as a quantifier, this matches one or more of preceeding sets of characters. In the firs bracket expression `[a-z0-9_\.-]` this would include characters a-z (case sensitive), numbers 0-9, underscore, period or hyphen. In the second bracket set `[\da-z\.-]`uses the quantifer to match any digit 0-9, a-z (case sensitive), period, or hyphen. The last quantifer is used in the last grouping where `{2,6}` matches a specified of atleast 2 but no more than 6 characters from the preceeding bracket expression `[a-z\.]`.

### Character Classes
The classes that are used in the expression are a character set with a range for number digit or letter from a-z. There is an escape character class incorporated searching for a dot notation. lastly the `\d` character class can found with seond grouping. This matches any digit character. 

### Grouping and Capturing
Parenthesis used within this expression capture a grouping of a string `(....)`. In this expression three groupings can be found. Later this can be used for extracting a subtring or using a back reference if needed. 

### Bracket Expressions
Three bracket expressions `[...]` can be found within this within each grouping. Within each set of brackets various character classes can be found. 

### Greedy Match
By default, the quantifer that allows the greedy match is `+`. This match will reference preceding characters as many times as possible. Towards the end of the expression `{2,6}` also tries to use its default greedy match by trying to match a minimum of two of the characters, but no more than six.


## Author

Adam Castro</br>
Github: https://github.com/avc0021</br>
Email: avc0021@gmail.com
