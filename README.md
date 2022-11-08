# Regex Email Tutorial

Regular expressions,also known as Regex, are combinations of special character operators. They are symbols that control the search using patterns.

## Summary

The regex pattern that we are looking at can be used to verify that user input is a valid email address:
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
The anchors in this expression has `^` and `$`, which means the expression will look for an exact string match. This also shows the beginning and the ending of the string.

### Quantifiers
The quantifiers within this expression includes the `+` and `{2,6}`. The `+` connects the email name, smail service, and domain name. The `{2,6}` will only allow a match range of 2 to 6 characters within the set of `[a-z\.]`.

### OR Operator
There are no or operators because there are no `|` within the expression.

### Character Classes
The character class is `\d`, it matches a single character that is a digit from `0-9`.

### Flags
Although this expression is between two `/`, the expression does not have any flags.

### Grouping and Capturing
The grouping and capturing would be the `()` in this regex. They capture the characters inside to be used as a subset. The first grouping will be `([a-z0-9_\.-]+)`.

### Bracket Expressions
The bracket expressions in this regex is `[]`. This expressions allows for multiple matches of the characters within the brackets. The bracket expressions are `[a-z0-9_\.-]`, `[\da-z\.-]`, `[a-z\.]`.

### Greedy and Lazy Match
This regrex includes greedy matches because it has the `+`. This expression will try to match as many times as possible to give back. 

### Boundaries
This expression has no boundaries. If it had `\b` at the beginning and at the end of the expression, it would perform a whole words only search.

### Back-references
This expression has no back-references. If it had `\1`, `\2`, `etc`, or `\k` it would mean that there is back-references.

### Look-ahead and Look-behind
This expression has no look-ahead orlLook-behind statements.

## Author
Josue Paniagua (https://github.com/josuepaniagua)
