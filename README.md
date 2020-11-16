# Validate Email Input (regex)

A regular expressions are characters used in forming any pattern of words or characters to search within any texts.They are very helpful in extracting any informations from texts.Most regular expressions pattern follow ASCII and sometimes uses unicode characters to match international texts.  

## Summary
Generally regular expressions are very helpfull in searching any pattern of characters ,their uses is not limited only in searching but also used on replacing the matched characters to desired ones.
Here we will demonestrate this regex pattern that matches valid email inputs from users. Email pattern should look like "solomon@gmail.com" as an example.

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

Anchors do not use to match any character at all. They use to match a positions like  after,before and between characters.

`^`matches right before the first character in the text. 
`$` matches position right after the last character in the text. 

### Quantifiers

Quantifiers in regular expression determines how many instances of a group, character or character class that must be present in the input for a match to be found in the text.
Here are some of the quantifiers used in our example.
    
`char+`    matches a string that has cha followed by one or more r

`char{2,6}`   matches a string that has cha followed by 2 up to 5 r

`c(har)*`   matches a string that has c followed by zero or more copies of the sequence har

`c(har){2,6}`  matches a string that has c followed by 2 up to 6 copies of the sequence har

### OR Operator
 
You can use or-operator to match a single character out of several possibly matching regular expressions.
OR operator has  lowest precedence of all regex operators. 
it tells the regex engine to match either everything to the left of "|",
or everything to the right of "|".Here are some OR-operators used in our example

`c(h|r)`   matches a string that has c followed by h or r and  capturing h or r

`c[hr]`   matches a string that has c followed by h or r but without capturing h or r

### Character Classes

A character class is a special pattern or notation that matches any character from a certain given string. Here are some used character class in our example.


`\d`         matches a single character that is a digit

`.`          matches any character 

### Flags

Slashes `/.../` informs  that we are defining a regular expression. Slashes play the same role as quotes for strings and at the end of those characters 
we can create a flag with these values

### Grouping and Capturing

Regex allow us to not only matching text but also to extract informations for further processing. This is done by defining groups of characters and capturing them using the  parentheses `(  )` .
Any pattern inside of the parentheses will be captured as a group. 
Like in our example this can be used to match  emails from all sorts of data.

### Bracket Expressions

Square brackets in regular expression `[ ]` designate a character class and match a single character in the text or string. Inside a character class,
only the character class metacharacters (backslash, circumflex anchor and hyphen) have special meaning.

`\`   general escape character

`^`   negate the class, if this is the first character in the brackets (If ^ is not the first, it is not a metacharacter.)


## Author

Solomon Meresa
[Github Profile](https://github.com/solomonmeresa)
