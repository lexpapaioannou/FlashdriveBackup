# FlashdriveBackup

# Synopsis
This script is designed to copy any new folders found in the user's /Volumes/ directory into a folder within the /Applications/ directory by use of the shutil.copytree function.  

It does this by first seeing if there is a directory already in place in the user's /Applications/ directory.  If there is, it will print a message saying that it is already there, otherwise it will print the location name of the directory created.  
The program then checks every second to see if there is a change within the user's /Volumes/ directory.  If a folder has been added, it will print a statment stating that it has detected a new folder and is beginning to copy it.  If a folder has been removed (i.e. a flashdrive has been unplugged), it will print a statement stating that it no longer detects the directory.
The program moves all packup files to a new folder each time, named after the name of the directory that was found in /Volumes/ followed by the date and time the program detected the external drive. (i.e. a flashdrive named "LexED" could create a folder called "LexED2017-02-15 15/56/03.720245")

AutobackupV2.py acts as the same as Autobackup.py, but will now display a spinning line while loading files.  This is to show that the program is still functioning while loading larger files.  This is done through use of threading and calling methods 

As of now this script only works on Mac OS.

# Motivation
This was a simple project for a friend and collegue of mine.  My friend requested a script that would automatically back up any files form a flashdrive onto a computer.

# Installation
Simply download the AutoBackupv2.py and run the script. 

# Tests
A flashdrive named "NO NAME" containing 1.74 GB was moved to "/Applications/autoBackup/NO NAME2018-01-24 16/22/08.944084" after roughly 3 minutes.

# License 
Copyright 2018 Alexander Papaioannou

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
