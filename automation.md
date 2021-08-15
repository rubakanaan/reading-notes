# Python Regular Expression

* Regular Expressions : often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not.
* They are used at the server side to validate the format of email addresses or passwords during registration, used for parsing text data files to find, replace, or delete certain string, etc. They help in manipulating textual data, which is often a prerequisite for data science projects involving text mining.
* if you want to start using them in your Python scripts, you have to do import re
* Ordinary characters are the simplest regular expressions. They match themselves exactly and do not have a special meaning in their regular expression syntax.
* Special characters are characters that do not match themselves as seen but have a special meaning when used in a regular expression. For simple understanding, they can be thought of as reserved metacharacters that denote something else and not what they look like.

<br> 

### Grouping in Regular Expressions
* The group feature of regular expression allows you to pick up parts of the matching text. Parts of a regular expression pattern bounded by parenthesis () are called groups. The parenthesis does not change what the expression matches, but rather forms groups within the matched sequence. You have been using the group() function all along in this tutorial's examples. The plain match.group() without any argument is still the whole matched text as usual.
<br>

### Greedy vs. Non-Greedy Matching

* When a special character matches as much of the search sequence (string) as possible, it is said to be a "Greedy Match"
* Although regular expressions are very powerful and helpful, be wary of long, confusing expressions that are hard for others, and also you to understand and maintain over time.
<br>

### Copying Files
* **copyfile() **: copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file.
* Because the function opens the input file for reading, regardless of its type, special files (such as Unix device nodes) cannot be copied as new special files with copyfile().
* The implementation of copyfile() uses the lower-level function copyfileobj(). While the arguments to copyfile() are filenames, the arguments to copyfileobj() are open file handles. The optional third argument is a buffer length to use for reading in blocks.
<br>

### Copying File Metadata
* By default when a new file is created under Unix, it receives permissions based on the umask of the current user. To copy the permissions from one file to another, use copymode().
<br>

### Finding Files
The **which()** function scans a search path looking for a named file. The typical use case is to find an executable program on the shell’s search path defined in the environment variable PATH.
<br>

### File System Space
It can be useful to examine the local file system to see how much space is available before performing a long running operation that may exhaust that space. disk_usage() returns a tuple with the total space, the amount currently being used, and the amount remaining free.