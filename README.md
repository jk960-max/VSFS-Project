# Project 1: Very Simple File System (VSFS)
Course: CIS 321 — Project 1  
Student: Joseph Kang

# Description of VSFS
Very Simple File System (VSFS) is a simplified file system used for educational goals to teach basic file systems concepts. It is a typical UNIX file system that has different types of data structures, access methods, and various policies that are in many file systems. It is pure software, not a CPU and memory visualization. There are disk blocks, data region, and allocation structures(free list), disk space (metadata, inodes, an inode table, superblock), and bitmaps. It operates by managing files and directories through a structure that maps file names to data blocks stored on disk. It monitors file locations and metadata through an inode table and a directory structure. 

# Description of my code
This project runs a VSFS using Python. I implemented directories, file creation, listing, and button class. Each structure is represented as a directory mapping names to objects such as make directory (mkdir), change directory (cd), and create file. I set up the GUI functions for text and file system and background color. I set up the buttons for the button actions that say like "Create Folder", "Create File", and "Go  Up".  

# Components that I used
-Inodes
-Bitmaps
-Data Block
-File
-File System
-Button Class
-GUI setup
-GUI functions
