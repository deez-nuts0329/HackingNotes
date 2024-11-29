## HackingNotes
- [Cracking Zip Files](#cracking-zip-files)
- [Using Dirb To Find Files](#using-dirb-to-find-files)
## Cracking Zip Files
Cracking Zip Files you need to use Zip2John
- Open the terminal and use zip2john -s zipfile.zip and export it to a .txt filelike this :
```bash
zip2john -s file.zip > zip.txt
```
- Then use john to crack it like this:
```bash
john zip.txt --wordlists wordlists.txt 
```
## Using Dirb To Find Files
To find hidden files in dirb you need to
```bash
dirb http://example.com/ -X .txt,.js,.py,.php
```
