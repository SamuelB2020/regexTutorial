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
