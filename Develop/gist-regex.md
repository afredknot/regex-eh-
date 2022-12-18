# Title (URL (regex) breakdown)

Welcome to your Regex ("Regular Expression") tutorial. 

To begin lets talk about what Regex is.
Regex is a sequence of characters that define a search pattern in a body of text. Regex takes a body of text and looks through the characters in it as a literal character/body. It is then able to take "meta character" which helps to define its search perameters. Meta characters are things such as "[a-z]" which Match range of characters specified by the hyphen, "." which matches any single character and also "\" which uses the literal meaning of the metacharacter or for basic regex, treat the next character as a metacharacter.

I hope you enjoy this walkthrough  and that it will bring a good sense of how a regex and its components work together to return what you're looking for.

## Summary

In this tutorial we will be going through the compnents of matching a  URL /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/ and why this regex is able to accompish its intended goal, how it happens, and why.

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

Anchors deleniate the beginning and end of our strings. With the ^ denoting the beginning of the string and the $ signals the end. This is something that you do not want to be forgetting seeing as how it gives the beginning and end points for the search perameters.

### Quantifiers

Now lets move on to quantifiers. Quantifiers indicate numbers of charaters or expressions to match.
For example /^(https?:\/\/) ... *\/?$/.
We will start with the ?. the ? used at the beginning of the string will match the preceding "s" either 0 or 1 times making it either look for http or https and give you back the correct output.

Next the {2,6} is looking to tell regex that there can only be 2 to 6 characters in this section of the url giving us a place to put the address direction in the url (ie. .com, .org, .gov)

Wrapping this section up we have the * which is able to match the preceeding items 0 or more times. At the end of the string we have 2. ([\/\w \.-]*)*\/?$/ 

These look at the file endpoint and since it is able to match the preceeding 0 or more times to reach the specific domain that we are looking for.

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

With the bracket expression we can indicate a set of characters to match and any of the individual characters betwixt these brackets will match i.e. [\da-z\.-]+)\.([a-z\.]. Often we will see either parts of the alphabet or numerals. In this case we have the alphabet .([a-z\.].

### Greedy and Lazy Match

Greedy matches are accomplished by default with the * or + symbols, since they are able to match the preceeding elements 0 or more times.

Lazy matches are accomplished by adding a ? before these afore mentioned greedy characters.

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

Daniel has been going through the full-stack coding bootcamp with OSU. Looking to break into the Web-Development scene with the experience of DEV OPS and Full-Stack coding sprints he has gained and will continue to develop through the years. 

Github Repository -- https://github.com/afredknot

LinkedIn Profile -- https://www.linkedin.com/in/daniel-nelson-3440b5b1/

Email -- afredknot@gmail.com
