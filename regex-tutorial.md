# Regular Expression (Regex) Tutorial

This tutorial will explain the basic fundamentals, components, and characteristics of Regular Expressions (Regex) while examining a use case for validating an email address. By the end of this tutorial, you should be able to explain the basics of Regex as well as be able to identify the compents that make up a Regex search statement.

## Summary

Throughout this tutorial, we will be referencing the following JavaScript regex that is used for validating email inputs in a form.

```
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
```

An email address is typically broken up into three disticnt parts: the 'user name', 'domain name', and 'domain extention'. The structure follows this pattern: `username`@`domainname`.`dx`

## Table of Contents

- [Boundaries](#boundaries)
- [Anchors](#anchors)
- [Bracket Expressions](#bracket-expressions)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)

## Regex Components

### Boundaries
To begin, we need to wrap our regex between '/' boundries. This creates the limits of our expression. All parameters will go between two '/' boundries.

### Anchors
Anchors are special types of boundries that indicate specifc positions within the expression. The first anchor we see in our expression is '^' immediately following the first boundry. This anchor indicates the start of a specified string. Its corresponding anchor is '$' which preceeds the final boundry and indicates the end of a string.

### Bracket Expressions
Bracket expressions dictate which portions of the expression can contain which specific sets of characters. What those characters are and how they are used are explained in the following sections.

### Quantifiers
The example regex shows two different types of quantifiers. The first we see is a '+' and the second is {...}. The plus (+) signifies a match for any characters found in the bracket expressions preceeding them. The brace ({...}) quantifier indcaites a range of matches (2 to 6 in this case) of the characters found in its preeceding bracket expression.

### Character Classes
Character classes are typically contained within bracket expressions but do not nessesarily need to be. The following are the character classes we see in the order found in our regex and their meanings:

`a-z`
>Used to match any letter within the range of lowercase letters.

`0-9`1
>Similarly used to match any number within the range.

`_`
>Used to match literal underscores.

`\.`
>Used to match dots (.). Because dots have a function in regex expressions, a '\' is used to indicate the character.

`-`
>Used to match literal hypens.

`\d`
>Effectively the same as 0-9.

`@`
>Used to match literal 'at' signs.

### Grouping and Capturing
Grouping constructs allow us to partition a regex into compenants meant to be matched one at a time. Capture groups are bounded by '(...)'.

## Author

Charlie (soulslurpee) is a Michigan based wannabe web-developer. Check out my work [here](https://github.com/soulslurpee/)
