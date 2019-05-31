# Markdown Tutorial Part 1: Regex in General

## What is a Regex?
 Simply a regex is a pattern to match characters or character combinations in a string. They are mainly used to remove characters or ccombinations or to search for them in a given string.

 In Javascript a regex is enclosed with forward slashes like

 <pre lang="js">var regularExpression = /[a-z]/;
</pre> 

they can also be written using object syntax

<pre lang="js">
var regularExpression = new RegExp('a-z');
</pre>

## Regex syntax
Regex as seen above is enclosed in a pair of //'s. This signifies the regex pattern, anything placed after the last / is a command that affects this.
For example
<pre lang="js">var x = x.replace(/[a-z]/g, "");</pre>
The g at the end makes this a global effector on the regex. This is a very important catch as you can globally replace things in JS.
<pre lang="js">var x = x.replace(/[a-z]/i, "");</pre>
The i after the regex pattern makes the match cas insensitive meaning it will replace all characters that match regardless of case.

<pre lang="js">var regex = /t*st/;</pre>
The use of a * character after a letter will match the preceding letter as many times as you want.
<pre lang="js">var regex = /.est/;</pre>
The use of the . character will match any character one time in the first section of the pattern.

<pre lang = "js">var regex = /\d/;</pre>
The use of the \d will match any integer, if you need to match multiple integers you can stack them on top of each other i.e. \d\d for two ints.
<pre lang = "js">var regex = /\D/;</pre>
The use of a capital D will match any non digit character
<pre lang = "js">var regex = /\w/;</pre>
The use of the w pattern match will make it so that it matches any word character
<pre lang = "js">var regex = /\W/;</pre>
Match any non word character
<pre lang = "js">var regex = /\s/;</pre>
This will match any white space character
#### Note *Using the capital will match the opposite for all of these pattern matching*

<pre lang = "js">var regex = /[x-y]/;</pre>
The use of square brackets allows the selecting of any characters inside them being matched. The use of a - will match a range from whatever is set i.e. a-z will match all charcters from a to z.

<pre lang = "js">var regex = /[abcd]efg/;</pre>
use the square brackets to match the start of a combination

<pre lang = "js">var regex = /something{x}/;</pre>
This can be used to match something x times you can put anyother characters in front.

<pre lang ="js">var regex = /(something)?/;</pre>
This will match the thing in the brackets if it exists.
