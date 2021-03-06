# Sublime-Build-Script-for-Contest-cpp-
A build script for Sublime Text 3 for C++ useful in contests (Competitive Programming)

## How to use?
Simply go to Tools > Build Systems > New Build System and paste the code in the [file](contest.sublime-build). Then select it in Tools > Build Systems and use `Ctrl+B` to compile and run.

## Options
Options/Variants can be selected using `Ctrl+Shift+B`
* The normal mode compiles and runs (outputs in builtin terminal)
* in ext shell: compiles and runs the code in an external shell (gnome terminal)
* with input file (in.txt): compile and runs the code taking input from an input file (in.txt) (has to be in same directory) instead of stdin (outputs in builtin terminal)
* with input (in.txt) and output (out.txt) file: run the code taking input from an input file (in.txt) and outputs in an output file (out.txt)

## Note
1. It is only tested for Linux (Ubuntu 18.x, 19.x) for Sublime Text 3. Should work for other linux distros. Can't say the same for windows.
2. The default C++ standard version is set to C++11, to change `-std=c++11` to whatever necessary. 
3. It uses the time command line utility to measure runtime. Change the `-f` option to change display format.
4. Default timeout is `5s`. To change, put your desired timeout in `timeout <timeout> time ...`.
