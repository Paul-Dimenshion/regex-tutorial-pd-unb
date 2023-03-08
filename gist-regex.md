# Regular expressions (REGEX)

In this gist we will talk about regular expressions in JavaScript (RegExp), and I will give you some frequently used examples. I’m not going to give you a definition of what it is, because there’s plenty of information on the Internet about it. I just want to give you a few examples so you can choose the right one.  It took me a long time to find a normal source where everything would be described in detail. For you personally, I will expedite this process by writing this little record.

## Summary

The following code will be used throughout the tutorial to give specific examples for how the components of regex can be used. The following code can be used for matching emails. One use for this code is that it can be used to validate to make sure that an email follows the correct format.

For this I will need the following regular expression:</br> 
`/\$\#([a-z0-9]{1,})\#\$/gi`</br>

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

Carriage `^` and dollar `$` symbols have special values in regular expressions. They are called "anchors" (anchors). The carriage `^` means a match with the beginning of the text, and the dollar `$` - with the end. For example, let’s check whether the text starts with `Mary`:

`let str1 = "Mary had a little lamb";`
`alert( /^Mary/.test(str1) ); // true`

 The template `^Mary` means: "the beginning of the line, then Mary". Similarly, you can check whether the string `snow` ends with `snow$`:

`let str1 = "it's fleece was white as snow";`
`alert( /snow$/.test(str1) ); // true`

In these particular cases, we could also use the `startsWith/endsWith` string methods. You should apply regular expressions when you need to test more.

### Quantifiers

Let’s take a string of the form `+1(903)-123-45-67` and find all the numbers in it. But now we are not interested in numbers individually, but in numbers: `1, 903, 123, 45, 67`. Number is a sequence of `1` or more digits `\d`. To indicate the number of repetitions, we need to add a quantifier.

The simplest quantifier is the number in curly brackets: `{n}`.

It is added to the character (or character class, or to the set `[...]` etc.) and specifies how many we need.

There are many ways to specify a quantity, for example:

Exact quantity: `{5}`
The pattern `\d{5}` represents exactly 5 digits, it is equivalent to `\d\d\d\d\d`.

The following example finds a five-digit number:

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

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
