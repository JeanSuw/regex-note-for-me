# Regex note for me

This is a note-to-self about Regex. The objective for this project is to create a tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does.

## Summary
Regex (or regexp) is regular expression. It's a sequence of characters that define a search pattern.

This regex tutorial is about matching a Hex value.
<br>`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`<br>
As you can see here, this expression is written using a combination of special characters and literal characters. The special ones is used to find patterns in strings while the literal ones are used to find the exact matches for the specific words or phases. 

I recommended looked through the table of contents to start off with how the characters are used.


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
They are type of assertion that allows you to do many things.
It helps you specify which characters you want to match.
<br>`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`</br>

* `^` is a **Caret**. It matches the position before the characters. In otherword it matches the beginning of the text
* `$` is a **Dollar sign**. It matches the position after the characters (which means matching at the end of the text)
* `/` is a **Front tick**. The one at the beginning is the open Front tick while the back is the close Front tick
### Quantifiers

* `?` Matches zero or one time.

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author
This tutorial is created by [JeanSuw](https://github.com/JeanSuw)