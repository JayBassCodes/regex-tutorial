# Title (replace with your title)

Regular Expressions and How to Use Them

## Summary

In this tutorial, I will be explaining how to use regular expressions. I will be explaining the different components of regular expressions and how to use them. I will be using the following regex as an example: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` which validates a hex value. 


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
breaking down the components of the above regex, we can see that it is made up of the following: [a-f0-9]{6} and [a-f0-9]{3}. The first component will search for a value of a-f, A-F, 0-9 and give 6 digits (eg. aBc458). The second component looks for the same letters and numbers but only spans 3 digits (eg. a45) 

### Anchors
Anchors are used to match a position before or after characters. The ^ anchor is used to match the beginning of a string. The $ anchor is used to match the end of a string. So in `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` the ^ anchor is used to match the beginning of the string and the $ anchor is used to match the end of the string.

### Quantifiers
The quantifiers used are *, ?, and {}. These describe how many digits to match. The * quantifier matches 0 or more of the preceding token. The ? quantifier matches 0 or 1 of the preceding token. The {} quantifier matches the specified quantity of the preceding token. So in `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` the {} quantifier is used to match 6 or 3 of the preceding token.

### Grouping Constructs
Grouping constructs are used to group tokens together and create subexpressions. In the above regex, the () grouping construct is used to group the two components together. In our example we have the 2 components grouped together and then the | operator is used to match either component. See the OR Operator section for more information.

### Bracket Expressions
Bracket expressions are used to match a single character out of a set of characters. In our example, the bracket expression is [a-f0-9]. This will match any character that is a-f, A-F, or 0-9.

### Character Classes
Character classes are used to match a single character out of a set of characters. In our example, the character class is [a-f0-9]. This will match any character that is a-f, A-F, or 0-9.

### The OR Operator
The OR operator is used to match either the expression before or after the operator. In our example, the OR operator is used to match either the first component or the second component.

### Flags
Flags are used to change the way the regex engine interprets the regex. In our example, the flags are ^ and $. The ^ flag is used to match the beginning of a string. The $ flag is used to match the end of a string.

### Character Escapes
Character escapes are used to match a character that has special meaning in regex. In our example, the character escape is \d. This will match any digit character.

## Author
Jacob Bassett

Jacob Bassett is a full-stack programmer with an interest in server-sided programming. I am currently learning the MERN stack through the University of Connecticut's coding bootcamp. 