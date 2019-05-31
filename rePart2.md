# Using Regex with Javascript

## What methods in Javascript allow Regular Expressions?

In Javascript there are 7 methods that are either called on regular expressions or a regular expression is a parameter to one of them. However there are only a few that are used frequently and are hence explained in this part.

The full list is as follows

|Name of Method|Description|
|--------------|------------
|exec|A RegExp method that executes a search for a match in a string. It returns an array of information or null.|
|test|A RegExp method that tests for a match in a string. It returns true or false.|
|match|A String method that executes a search for a match in a string. It returns an array of information or null.
|matchAll|A String method that returns an iterator containing all of the matches, including capturing groups.|
|search|A String method that tests for a match in a string. It returns the index of the match, or -1 if the search fails.|
|replace|A String method that executes a search for a match in a string, and replaces the matched substring with a replacement substring.|
|split|A String method that uses a regular expression or a fixed string to break a string into an array of substrings.|

Source: <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">Mozilla MDN Web</a>


## The Test Method

For the test method the method is called on the regular expression not the string.

For example
<pre>
var re = /[A-Z]/g;
boscode.display(re.test("hello"));
// => false
</pre>

The test method tests whether a match could be found on a string and returns a boolean value either true or false.
It is useful for tasks that require a test to see whether a string conforms to a certain specification or standard.

## The Replace Method

One of the most common uses for a regular expression in Javascript is to replace characters within a given string.
Consider the following: you are to replace every instance of a vowel character within a string to a "#" character, In normal javascript without regular expressions the code would look something like it is 11 lines of code.

<pre lang="js">
function replaceVowel(string){
  var newString = "";
  for (let i = 0; i < string.length; i++) {
    if (string[i] == "a" || string[i] == "e" || string[i] == "i" || string[i] == "o" || string[i] == "u"){
    newString+= "#";
    }
    else{
      newString += string[i]
    }
  }
  return newString
}
</pre>

With a regular expression we need to create a pattern to match every instance of a vowel. This is simply achieved by creating a list of all vowel characters.

<pre lang="js">
var pattern = /[aeiou]/g
</pre>

Now we can convert the above 11 line code to 3 lines of code.

<pre lang="js">
function replaceVowel(string) {
  return string.replace(/[aeiou]/g,"#");
}
</pre>

## The Search Method

The search method allows for a programmer to get details on where the match has been found exactly.

Consider the following

<pre lang="js">
var str = "hey MatE";
boscode.display(str.search(/[A-Z]]/g)); // => 4, as this is the location of the first capital letter
</pre>




