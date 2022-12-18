# Regex Tutorial for Matching an Email Address

This tutorial explains how to use a regex in order to match email address with the expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
This helps validating emails in many diffrent application.

## Summary

Regular expressions, (a.k.a regex), are a series of special characters that define a search pattern. This is commonly used to find patterns within a string, find/replace characters within a string or validate input. In this tutortial, we walk you through the components of a regex using to match an email.


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

The anchors used in this regex expression for matching an email are "^" and "$".
"^" indicates the beginning of the string.
"$" indicates the ending of the string. 

This regex ends at $ while the Multiline, (m), is not enabled.

### Quantifiers

Quantifiers in this regex are "+" and "{2,6}"

"+" operator connects the users email name + @domain service name + .com 
"{2,6}" allows a match between 2 upto 6 characters for the character set of lower case "a" to "z" and "."

### Grouping Constructs

Group #1 is ([a-z0-9_\.-]+) that matches the user name
Group #2 is ([\da-z\.-]+) that matches the email domain name
Group #3 is ([a-z\.]{2,6}) that matches the email top-level domain, domain type, such as ".com"

### Bracket Expressions

Bracked expressios for email validation includes the character sets of 

[a-z0-9_\.-] matches any letter a-z (case senstive), a character 0-9, and the characters "_" , "-" , and "." 
[\da-z\.-] matches a single digit from 0-9, any character a-z (case senstive), and the characters "." and "-"
[a-z\.] matches any character a-z (case senstive) and the character "."

### Character Classes

The character class in this expression is "\d"
"\d" matches a single digit from "0" to "9" 
It only matches a single digit such as "9", but not "99"

### The OR Operator

### Flags

### Character Escapes

### Greedy and Lazy Match
The greedy matches used in this regex expression are Quantifier "+" and "{}"

So, it will match as many times as possible giving back as needed "+" and also  matching "{2,6}" for the last capture group.

## Author

John Aslani is Data Scientist and please find further information on [my GitHub](https://github.com/johnaslani) or [Regex-Tutorial](https://github.com/johnaslani/Regex-Tutorial)


Should you have any questions, please reach me at [aslani.john@gmail.com](mailto:aslani.john@gmail.com)

