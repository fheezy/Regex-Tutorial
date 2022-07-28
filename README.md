# Regex-Tutorial

Regex is a search pattern (a set of symbols) that helps you match, locate and manage text – making it easier to extract information from code, log files, spreadsheets and documents.

## Summary

In this tutorial, we will be going over regex and the break down of an email regex specfically. Regex it self is broken down into several catagories which we will go over all that regualtes towards an email regex, starting with Anchors to Greedy and Lazy Match.
we will learn how this regex '/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/' to this email fh23@gmail.com 

## Table of Contents

- [Regex Tutorial](#regex-tutorial)
- [Summary](#summary)
- [Table of Contents](#table-of-contents)
- [Regex Components](#regex-components)
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Author](#author)

## Regex Components

A regex is considered a literal, so the pattern must be wrapped in slash characters (/).

### Anchors

The characters "^" and "$" are both considered to be anchors. The "$" anchor signifies a string that ends with the characters that precede it. Just as with the "^" character, it can be preceded by an exact string or a range of possible matches. Regarding in this case, we have '/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/' 
"^" is called the caret anchor singling the computer to know its the beginning of the text while "$" is the dollar anchor and it signifies the end of a text.
As we go down this tutorial we will go over what's in between the anchors !

### Quantifiers

Quantifiers set the limits of the string that your regex matches (or an individual section of the string). They frequently include the minimum and maximum number of characters that your regex is looking for. Typically include: "*"-Matches the pattern zero or more times, "+"-Matches the pattern one or more times, "?"-Matches the pattern zero or one time, and "{}" which can be provided in three different ways. Regarding to our regex '/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/',
the quantifiers will be "{2,6}" although the bracket expression is "[a-z\.]" so this means the string can be 2 and 6 characters containing lowercase a-z charcaters as well "." which is after "\" letting the computer know that the "." goes after. 

### OR Operator

### Character Classes

A character class in a regex defines a set of characters, any one of which can occur in an input string to fulfill a match.

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match


## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
