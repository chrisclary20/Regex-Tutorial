## Regex Tutorial by Christopher Clary 
**Regular expressions, or ReGex, helps define search patterns that can then be used to look for certain special characters or formats within an input string. In this tutorial, I will be explaining how ReGex is used and implemented by going over each component of a ReGex expression and explaining how it functions!**

## Table of Contents

 - [Summary](#summary)
 - [Components of ReGex](#components-of-regex)
 - [Author](#author)
 - [Sources](#sources)

## Summary
As stated previously, ReGex helps define search patterns so we can then look for special characters or formats within an input string. This is useful, for example, if we were to check for whether a username can be valid within our webpage, or if we were to look for valid characters within an email address. For another example, if our ReGex were set to define "Hello", this would then match any string that contains the input string of "Hello".

## Components of ReGex

  **Character Classes**
  
 - /d and /w are common ways to find either digits or common letters from the Latin alphabet.           
`const statement = "Hello World!";
const regexStatement = /\w/g;
console.log(statement.match(regexStatement));`
The code in this example would output an array of the letters used in the initial statement variable like so - ``> Array ["H", "e", "l", "l", "o", "W", "o", "r", "l", "d"]``

**Quantifiers**

 - Quantifiers match a number of instances of a character, group, or [character class](https://www.javascripttutorial.net/javascript-character-classes/) in a string. [Source: https://www.javascripttutorial.net/regular-expression-quantifiers/] 
 For example, `const year = "We are in 2021"; const defineYear = year.match(/\d{4}); console.log(defineYear);` The quantifier in this code can be seen at ``/\d{4}`` where the {4} is stating that we want to match a four-digit number. The expected output will be `2021`.

**Anchors**

 - An anchor matches a position before, after, or between characters and is signaled using ^ (*starting anchor*) and $ (*closing anchor*).

**Capturing Groups**

 - Group capturing allows us to get part of a match as a separate item within the result array.

**Backreferencing**

 - Backreferencing allows us to grab input from capturing groups to then be used later on.
 
 **Character Escapes**
 
 - We can use a backslash ("\") to denote that we want to search for a special character without that character being presumed a searching mechanism.

## Author

This tutorial was created by Christopher Clary using Slack Edit [slackedit.io]. 

## Sources

 - https://cs.lmu.edu/~ray/notes/regex/
 - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions/Character_Classes
 - https://javascript.info/regexp-groups
 - https://www.regular-expressions.info/backref.html
 



 

