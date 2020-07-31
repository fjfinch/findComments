# findComments
This script searches for comments on webpages source code. (The low-hanging fruit in CTFs). It needs a file with curlable pages as an argument. Use this script simultaneously besides a web content scanner (ex. gobuster,dirbuster,dirsearch). Of which the scanner should give its output to this scripts input.
Ex.     `gobuster dir -u <IP> -w <WORDLIST> -en -o pages.txt`
        `findComments pages.txt`
Or use the script with a pre made file with pages in it. Make sure the output is curlable.
Because the script is made to be run besides a program, it wil not end. So use CTRL+C to stop the script.

## Context
When doing Cyber Security CTFs (Capture the flags), you might end up working with a webserver. Sometimes there are comments left behind in the source code containing important info. This is really low-hanging fruit, and it is annoying to check every webpage. So a script it is.

## How to
### Dependencies
This script uses `curl` to find the webpages source code.

### Usage
Usage: findComments <FILE>
where <FILE> is a file containing curlable webpages. You can make the file yourself, of you can run this script simultaneously with a web scanner like gobuster.

![Script with gobuster](https://imgur.com/AkCe6W7.png)


## ToDO
I might include threading/parallel curling, to make this script faster, at some point.
Also I might make a Python version.
