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

A character class in a regex defines a set of characters, any one of which can occur in an input string to fulfill a match. Here are some common character classes: 
"."—Matches any character except the newline character (\n)

"\d"—Matches any Arabic numeral digit. This class is equivalent to the bracket expression [0-9].

"\w"—Matches any alphanumeric character from the basic Latin alphabet, including the underscore (_). This class is equivalent to the bracket expression [A-Za-z0-9_].

"\s"—Matches a single whitespace character, including tabs and line breaks.
However in this regex, you can see that we have a "\d" therefore this character can be defined with a single digit or from 0-9.

### Flags

Flags are placed at the end of a regex, after the second slash, and they define additional functionality or limits for the regex. Out of the 6 optional flags that can be used, the 3 most common you'll encounter are: 
"g"—Global search: the regex should be tested against all possible matches in a string.

"i"—Case-insensitive search: case should be ignored while attempting a match in a string

"m"—Multi-line search: a multi-line input string should be treated as multiple lines 

### Grouping and Capturing

Capturing groups are a way to treat multiple characters as a single unit. They are created by placing the characters to be grouped inside a set of parentheses. In simple terms it is dividing the arrays with "()" but in this case our email regex '/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/' has 3 groups ([a-z0-9_\.-]+), ([\da-z\.-]+), and ([a-z\.]{2,6}). Between the three groups you can see that the "@" and "." which indicates that its an email regex, the first group is right before the "@" and after will be provided witht the provider and after the "." will end with three characters.

### Bracket Expressions

Anything inside a set of square brackets ([]) represents a range of characters that we want to match. These patterns are known as bracket expressions, but they are also known as a positive character group, because they outline the characters we want to include. In regards in this regex, the bracket expression would be "[a-z0-9] therefore leading the computer to search any characters between a-z and any digit between 0-9.

## Author

Farhan Hoque [Github](https://github.com/fheezy)