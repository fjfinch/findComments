# findComments
This script searches for comments on webpages source code. (The low-hanging fruit in CTFs). It needs a file with curlable pages as an argument.

```bash
findComments pages.txt
```

## Context
When doing InfoSec/CyberSec capture the flags, you might end up enumerating a webserver. Sometimes there are comments left behind in the source code containing important info. This is really low-hanging fruit, and it is annoying to check every webpage. So a script it issss.

## How to use?
This script is made on/for (Debian) Kali Linux and uses `curl` to find the webpages source code.

Usage: `findComments <FILE>`

Where \<FILE\> is a file containing curlable webpages.
