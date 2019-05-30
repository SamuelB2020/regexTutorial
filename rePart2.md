# Using Regex with Javascript



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

