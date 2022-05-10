# USING REGEX TO DETECT A HEX VALUE

## Summary

QUESTION: How to detect a HEX value in RegEx?
SOLUTION: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

*** NOTE PLEASE READ THE BELOW FOR FULL EXPLINATION OF THE SOLUTION ***

## Table of Contents

- [Regex Components](#regex-components)
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)

### Regex Components

Please see the breakdown of the comonents needed for this RegEx Expression :)

( ) = using parenthesis groups components together
[ ] = brackets lets you specify unique characters allowed
 -  = the dash sets a range of values
{ } = curlies let you set a range or quantity of allowed components
 |  = pipes are equivalent to an "OR" statement

### Anchors

Anchors are used to force a statement to work from the start or end of the expression

 ^  = requires validation from the first position
 $  = The dollar sign means the matching stops at the end of the string
 
### Quantifiers

 ?  = This allows Zero or One times of the specified component
{ } = This specifies a quantity of items

### Grouping Constructs

Grouping allows us to allow multiple solutions to pass validation...
In our Solution you can see the 2 groupings:
GROUP 1: [a-f0-9]{6}
GROUP 2: [a-f0-9]{3}

### Bracket Expressions

As you can see in the Grouping section above... the brackets tell RegEx how many of each option is allowed

GROUP 1: [a-f0-9]{6} = Should have 6 valid characters in sequence
GROUP 2: [a-f0-9]{3} = Should have 3 valid characters in sequence

## Author
Rachel Leboeuf

// You are required to submit the following for review:
// The URL of the GitHub gist. Give the gist a unique name.