# Find Commands

# *Find* Command in Linux

Find is used for Finding something quickly with some data like type, name and size of the file.

**Syntax** : find *.or/* *-type* {-file or directory} *-name* {file-name or *.txt}* -iname* {for case sensitive} *-size* {for the size of file}

### To find all directories whose name contain the word *hacker*

### Syntax :- find / -type d -name *hacker* ====%% Put hacker inside the ** these for the special name. %% ====

The username of the owner of a file is specified with the user *-user*

- *size* is for specify the size ## Permissions — [[Pasted image 20210906173657.png]]

## ### finding by Time

For time-related there are two prefixes : *min* – for hours *time* – for days

There are three prefixes :

**accessed** => *-a* **modified** => *-m* **changed** => *-c*

> Ex - A file is modified more than 30 minutes ago :  -mmin +30
> 

> Ex - A file is accessed less than 7 days ago :  -atime -7
> 

> When you want to specify that the file was modified within last 24 hours the option is -mtime 0.
> 
- **newermt** 2020-03-03 => Find the file newer than 2020-03-03