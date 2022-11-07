# Class 17
### Automation
### Python Regex Tutorial
* Regular Expressions, often shortened to Regex is a series of characters used to check if a pattern exists within a string.
Search Engines, Search and Replace tools for word processors, and other similar things use something similar to Regex.
* Regex has a number of functions that can be used such as;
compile()
search()
findall()
sub()
split()
and more.
* To use Regex in Python, you start of by using the code import re to import Regex as a module.
* The most basic usage of Regex is with an ordinary character pattern. It is often used to find a literal set of character, "Tree" would search for the string "Tree" in the string you provide it.
* Once you get into special characters is when Regex really begins to open up. They are essentially reserved meta characters that mean something specific. For example;

^ means the start of the string
$ means the end of the string
[] matches any single character contained within the brackets;
[a,b,c] would match a, b, or c.
[a-zA-Z0-9] would match any single character a-z, A-Z, or 0-9.
The most diverse character is \ which is used to;
When used with a escape character following it, it will take on the special meaning of the term.
If the following character is not an escape character, it will be read as any other character
If can be used in front of meta-characters to remove their meta meaning and have them be read literally.
Some of the pre-defined sequences are;
\w for any letter,digit,or underscore
\W to mean anything else
\s for any whitespace character such as a space, newline, tab or return
\S for anything else
\d for any digit 0-9
\D for anything not a digit
You can also use repetitions to shorten up and further customize the Regex.
The use of + is to indicate repetition for the previous character or sequence one or more times from that position.
* for zero or more times from the position
? for zero or one times from that position
To check for a specific number of repetitions use square brackets, {}.
You can also group parts of the text with parentheses, ()
Patterns cab also be greedy or non-greedy.
You can also add flags to further change the behavior of Regex;
I for case-insensitive matches
S for allowing . to match any character including newline
M to allows the start of string and end of string to also mean newlines
X for verbose to allow for comments and whitespace in the regex expression