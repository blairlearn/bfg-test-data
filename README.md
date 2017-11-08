To reproduce the problem, follow these steps:

1. Clone this repository with the command `git clone --mirror https://github.com/blairlearn/bfg-test-data`
2. Copy replace.txt to the current directory.
3. Execute bfg-repo-cleaner with the command `java -jar bfg-1.12.16.jar --replace-text replace.txt --no-blob-protection bfg-test-data`

The files UCS-2-BE.txt and UCS-2-LE.txt will be unaltered.

Contents of this repository:

* ANSI.txt -- contains ANSI encoded text.
* UTF8.txt -- contains UTF8 encoded text.
* UCS-2-BE.txt -- contains UCS-2 (Big Endian) encoded text.
* UCS-2-LE.txt -- contains UCS-2 (Little Endian) encoded text.
* replace.txt -- string replacement pattern for the bfg-repo-cleaner.
* README.md -- this file.
