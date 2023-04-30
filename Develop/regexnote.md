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
They are used to quantify how many times a part of your regular expression should be repeated.
To use a quantifer you must add its symbols after a character (the characters can be a character class or a sub-expression). Every quantifiers have range, each symbols below will explains what they do.

* `?` Matches zero or one time.
* `x{6}`: In this expression, its means regex will match exactly 6 'x' characters. 
    * If we applied [a-f0-9] to 'x', like [a-f0-9]{6}, it means that regex will match 4 of [a-f0-9]
    * We can also rewrite it as [a-f0-9]{6,6} In other word repeat from 6 to 6 times. Repeat from N to N time
    * We also have another [a-f0-9] on the other side of |. However it ask to matches 3 times.
### OR Operator
"Or" or "|" is used to separate the terms inside the parenthesis (...)
<br>`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`</br>
In  this scenario, inside the parenthesis, we have regex matches 6  time of a-f0-9 or matches 3 times of a-f0-9.

### Character Classes
It is also called character sets.
* If you put random letters inside the bracket, it will match with any words that has one of letters inside the bracket
    * gr[ae]y will match either gray or grey
* But if you put a hyphen (this symbol: -) inside a character class then you are able to specify the range
    * In this case, [a-f0-9], you can add more range. 
    * There are two ranges in this square brackets
        * a-f means matches the character from a to f. The char code is 97 to 109.
        * 0-9 means matches the characters in range 0 to 9. The char code is 48 to 57.
<br>`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`</br>

### Flags
No flags in this line: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`
### Grouping and Capturing
Capturing is a way to treat multiple characters as a single unit.
In this case, the "[a-f0-9]{6}|[a-f0-9]{3}" is the substring.
### Bracket Expressions
It is used to match a single character or collating element.


### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author
This tutorial is created by [JeanSuw](https://github.com/JeanSuw)

## Links to form this tutorial
* [Quantifiers](https://blog.robertelder.org/regular-expression-quantifiers/#:~:text=%7BN%2C%7D%3F&text=%7BN%2CM%7D%3F&text=Quantifiers%20are%20used%20to%20quantify,times%20it%20should%20be%20repeated.)
* [Or](https://www.ocpsoft.org/tutorials/regular-expressions/or-in-regex/)
* [Character classes](https://www.regular-expressions.info/charclass.html)
* [Capturing Groups](https://docs.oracle.com/javase/tutorial/essential/regex/groups.html)
* [Capture Group Numbering & Naming: The Gory Details](https://www.rexegg.com/regex-capture.html)
* []()
* []()
* []()