# Exercises  with Regular Expressions

## Structure of exercises
Exercises are structured based on the following system 

<b> 1.XX</b> - These are basic exercises designed to build an understanding on constructing basic regular expressions and using them.

<b>2.XX</b> - These are intermediate exercises that require the use of other code apart from regular expression to solve a task. These tasks are designed to build familiarity with regular expressions within general JavaScript code.


<b>3.XX</b> - These are links to former ProgComp tasks or derivative tasks of similar difficulty that can be solved very efficiently using a regular expression. These tasks provide a practical use for regular expressions within a competitive programming context.

# 1.1: Does not exist

Given a string check whether it contains the character 'd' (case insensitive) if it does print the string and "does exist" or if it does not print "does not exist"

Example Input

<pre>
Test Dharcter
dtaa stuff
working code
this is stuff
the quick brown fox jumps over the dark cave
</pre>

Example output
<pre>
Test Dharcter - does exist
dtaa stuff - does exist
working code - does exist
this is stuff - does exist
the quick brown fox jumps over the dark cave - does exist
</pre>



## 1.2: Now I know my abc's

### Part A: Pre-Regex
Given a string from the console check whether it contains the substring 'abc' (case sensitive) if it does print the string alongside either true or false.

Example Input
<pre>
abdc
abcdwe
892jsls
gshabcjsabeabc</pre>
Example Output
<pre>
abdc - false
abcdwe - true
892jsls - false
gshabcjsabeabc - true
</pre>

### Part B: Regex Enlightenment

Implement the above part this time using a regular expression. The example inputs and outputs should work for both parts. 

Hint: The second part of this task can be achieved in 5 lines or under including the require at the top.


## 1.3: Syntax Error
Ah, the semicolon the bane of most programmers, semicolons in most languages are required at the end of lines of code to signify their end. Javascript thank goodness isn't one of these languages so your safe there.


Your task is to work out if a string entered in through the console ends in a semicolon. If it does print the code and "Correct" separated by a hyphen. If it does not, tell the programmer. Print the code and the string "Your code is incorrect" separated by a hyphen.

Input
<pre>
var test = 0
test++;
test = 9;
console.log(HELP ME);
code.write("data")
code.write("DRY Code");
</pre>

Output
<pre>
var test = 0 - Your code is incorrect
test++; - Correct
test = 9; - Correct
console.log(HELP ME); - Correct
code.write("data") - Your code is incorrect
code.write("DRY Code"); - Correct
</pre>

## 2.1: MAC48 Address Verifier
A media access control address is commonly used within networking applications, it is a unique identifier assigned to network interface controllers in a computer system. See <a href="https://en.wikipedia.org/wiki/MAC_address">MAC Address</a> for further information about their use.

All MAC addresses in IEEE 802 format have 6 sets of hexadecimal numbers separated by a hyphen for example the following.
<pre>
90-1B-63-84-43-E6
</pre>

Your Task is to read from a textfile and check whether the strings conform to the above formatting rules as set by IEEE 802. You should print either "Correct" or "Incorrect" following the input separated by a hyphen.

Input
<pre>
90-1B-63-84-43-E6
9A-AB-66-9D-4A-B6
I am definitely not a mac-address
WET code works 07-E3
90-1B-63-84-43-E6 WRONG
0F-37-2B-D5-4E-F4
91-69-3B-5G-C7-23
8E-0B-GG-M8-87-75
44-52-59-20-43-6F-64-65
83-28-323-2-1
</pre>

Output
<pre>
90-1B-63-84-43-E6 - Correct
9A-AB-66-9D-4A-B6 - Correct
I am definitely not a mac-address - Incorrect
WET code works 07-E3 - Incorrect
90-1B-63-84-43-E6 WRONG - Incorrect
0F-37-2B-D5-4E-F4 - Correct
91-69-3B-5G-C7-23 - Incorrect
8E-0B-GG-M8-87-75 - Incorrect
44-52-59-20-43-6F-64-65 - Incorrect
83-28-323-2-1 - Incorrect
</pre>
## 2.2: Is a correct sentence

A correct sentence in this context is a sentence that begins with a capital letter and ends in either a full stop, question mark or exclamation mark. 

Write a program that determines whether a given string matches these criteria and output the result to the console.

Input
<pre>
i can engrish
This is correctly formed prose.
incorrecly form of sentence.
To be, or not to be, that is the question.
lets stop here, that is a good idea
</pre>

Output
<pre>
i can engrish - Incorrect
This is correctly formed prose. - Correct
incorrecly form of sentence. - Incorrect
To be, or not to be, that is the question. - Correct
lets stop here, that is a good idea - Incorrect
</pre>


## 3.1: Digital Extraction

Please see task 1 in the following link to the 2009 ProgComp Competition

<a href="http://cgi.cse.unsw.edu.au/~progcomp/pop.php?loc=2009opentasks#task1">Task Link</a>


## 3.2: Pangrams

Please see task 2 in the following link to the 2012 ProgComp Competition

<a href="http://cgi.cse.unsw.edu.au/~progcomp/pop.php?loc=2012opentasks#task2">Task Link</a>



