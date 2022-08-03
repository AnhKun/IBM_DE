# Hands-on introduction to Linux commands and Shell scripting
- Navigating directories: cd

|Symbol|Stands for        |
|------|------------------|
|~     |Home directory    |
|/     |Root directory    |
|.     |Current directory |
|..    |Parent directory  |

**Some common shell commands for getting information include:**
- whoami - username
- id - user ID and group ID
- uname - operating system name
- ps - running processes
- top - resource usage
- df - mounted file systems
- man - reference manual
```
man id
```
- date - today's date
```
# displays the current date and time
date   
# displays the current date in mm/dd/yy format
date "+%D"

# Some of the popular format specifiers:
|Specifier | Explanation                                      |
|----------|--------------------------------------------------|
|%d        | Display the day of the month (01 to 31)          |
|%h        | Displays the abbreviated month name (Jan to Dec) |
|%m        | Displays the month of year (01 to 12)            |
|%Y        | Displays the four-digit year                     |
|%T        | Displays the time in 24 hour format as HH:MM:SS  |
|%H        | Displays the hour                                |
```

**Some common shell commands for working with files include:**
- cp - copy file
```
# to copy files:
cp /source/file  /dest/filename
cp /source/file  /dest/
# to copy directories:
cp -r /source/dir/  /dest/dir/
```
- mv - change file name or path
```
# to move files:
mv /source/file  /dest/dir/
# to move directories:
mv /source/dir/  /dest/dir/
```
- rm - remove file
```
rm folder1       # delete empty folder1
rm -r folder 1   # delete folder1 along with all its child's files objects
```
- touch - create empty file, update file timestamp
- chmod - change/modify file permissions
- wc - get count of lines, words, characters in file
- grep - return lines in file matching pattern

**Very common shell commands for navigating and working with directories include:**
- ls - list files and directories
```
ls -l   # include attributes like permissions, owner, size, and last-modified date
```
- find - find files in directory tree
```
find . -name "a.txt"   # find a specific file (a.txt) in current directory (.)
```
- pwd - get present working directory
- mkdir - make directory
- cd - change directory
- rmdir - remove directory

**For printing file contents or strings, common commands include:**
- cat - print entire file contents
- more - print file contents page-by-page
- head - print first N lines of file
```
head a.text        # print first 10 lines of file
head -n 3 a.text   # print first 3 lines of file
```
- tail - print last N lines of file
- echo - print string or variable value
```
echo "Hello World"
# Use the -e option of the echo command when working with special characters
echo -e "This will be printed \nin two lines"
```
- grep - ("global regular expression print") - return lines in file matching pattern

**Shell commands related to file compression and archiving applications include:**
- tar - archive a set of files
- zip - compress a set of files
- unzip - extract files from a compressed zip archive

Networking applications include the following:
- hostname - print hostname
- ping - send packets to URL and print response
- ifconfig - display or configure system network interfaces
- curl - display contents of file at a URL
- wget - download file from URL