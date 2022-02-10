# Week 17 Regex Tutorial

This is a Regex tutorial. The goal of this is to help users understand character syntax when reading regex lines.

## Summary

A Regex (short for regular expression) is a string of text that allows you to create patterns that help match, locate, and manage text.
Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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
Regex lines are literal, so be sure to wrap your code in forward slash characters (`/`). 

### Anchors
Anchors include ^ and $. <br/> 
'^' denotes the beginning of a string. <br/>
'$' denotes the end of a string. <br/>

### Quantifiers
Eager (Greedy and Generous) — match as much as possible, but give back. <br/>
i.e. '\w+\d\d\w+'  matches abcdef42skjhfskjfhsjdfs but inefficiently <br/>
Possessive — match as much as possible, but do NOT give back. <br/>
i.e. '\w++\d\d\w+'  does not match abcdef42skjhfskjfhsjdfs but is efficient<br/>
Reluctant — match as little as possible. <br/>
i.e. '\w+?\d\d\w+'  matches abcdef42skjhfskjfhsjdfs efficiently <br/>

### Grouping Constructs
Groups combine token sequences in order for them to operate together. For example, `(https?:\/\/)` which will match with "https://"
<br/>

### Bracket Expressions
Characters set within (`[]`) represent a range of characters that will try to be matched. We can write these expressions to include all of the characters we want to match. Examples: `[a-z]` and `[0-9]`
<br/>

### Character Classes
Specific characters from sets are called character classes. There are myriad character classes that are ready made. Examples: `\w` and `\d`. You can also make your own. <br/>

### The OR Operator

### Flags

### Character Escapes
The backslash character ('\') in Regex allows any characters that precede it to be read as a literal character. The backslash however loses it's functionality when it's inside of a bracket expression.
<br/>

### Example Walkthrough
---
<br/>
<br/>

**`(`** - opening of second grouping “[\da-z\.-]+”

**`[`** - opening of character set “\da-z\.-“

**`\d`** - matches any digit (0-9)

**`a-z`** - matches any alpha character in the range a-z. Case sensitive.

**`\.-`** - escape character followed by matches of characters “.” and “-“

**`]`** - closing of character set

**`+`** - indicates one or more occurrences of the preceding element. 

**`)`** - closing of second grouping

**`\.`** - escape character followed by a character match “.” 

<br />
## Second piece of URL
<br/>
<br/>
URL: https:// www .test. com/ about-us/ our-team
<br/>
Syntax: `([\da-z\.-]+)\.`

`(` - opening of second grouping “[\da-z\.-]+”

`[` - opening of character set “\da-z\.-“

`\d` - matches any digit (0-9)

`a-z` - matches any alpha character in the range a-z. Case sensitive.

`\.-` - escape character followed by matches of characters “.” and “-“

`]` - closing of character set

`+` - indicates one or more occurrences of the preceding element. 

`)` - closing of second grouping

**`\.` - escape character followed by a character match “.” 

<br />





## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
