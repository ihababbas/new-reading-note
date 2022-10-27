# class 04
## Reading and Writing Files in Python

### What Is a File?

File Paths
When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file. It’s broken up into three major parts: Folder Path, File Name and Extension

Line Endings
One problem often encountered when working with file data is the representation of a new line or line ending

Character Encodings
Another common problem that you may face is the encoding of the byte data. An encoding is a translation from byte data to human readable characters. This is typically done by assigning a numerical value to represent a character. The two most common encodings are the ASCII and UNICODE Formats. ASCII can only store 128 characters, while Unicode can contain up to 1,114,112 characters


### Opening and Closing a File in Python
Text File Types
A text file is the most common file that you’ll encounter. Here are some examples of how these files are opened:
open('abc.txt')
open('abc.txt', 'r')
open('abc.txt', 'w')

Buffered Binary File Types
A buffered binary file type is used for reading and writing binary files. Here are some examples of how these files are opened:
open('abc.txt', 'rb')
open('abc.txt', 'wb')

Raw File Types
A raw file type is:
“generally used as a low-level building-block for binary and text streams.”
It is therefore not typically used.

### Reading and Writing Opened Files

Iterating Over Each Line in the File

Working With Bytes

A Full Example: dos2unix.py
### Tips and Tricks
__file__

Appending to a File
Sometimes, you may want to append to a file or start writing at the end of an already populated file

Working With Two Files at the Same Time
There are times when you may want to read a file and write to another file at the same time.

Creating Your Own Context Manager
There may come a time when you’ll need finer control of the file object by placing it inside a custom class. When you do this, using the with statement can no longer be used unless you add a few magic methods: __enter__ and __exit__. By adding these, you’ll have created what’s called a context manager.
### Don’t Re-Invent the Snake
There are common situations that you may encounter while working with files. Most of these cases can be handled using other modules. Two common file types you may need to work with are .csv and .json. 