# Project 1: Virtual Simple File System (VSFS)
**Course:** CIS 321 — Project 1  
**Student:** Joseph Kang

## Overview
This project implements a simplified virtual file system (VSFS) following Chapter 40, *Three Easy Pieces*. The simulation includes a superblock, inode table, directory tree, free-space bitmap, data block simulation, and basic file/directory operations. A small Pygame GUI visually displays inodes, data blocks, and inode metadata.

## Files
- `inode.py` — `Inode` class (id, size, blocks)
- `bitmap.py` — `Bitmap` class (allocate/free blocks)
- `directory.py` — `Directory` class (nested dicts, cd/ls/mkdir)
- `filesystem.py` — `FileSystem` class integrating everything (create/read/write/rm)
- `gui.py` — Pygame frontend showing directory, inode info, and bitmap
- `main.py` — Demo runner (CLI + optional GUI toggle)
- `explanation_video.mp4` — demonstration video of program running

## Implemented Components (Chapter 40)
- Superblock: implemented as dictionary in `FileSystem`. ✔
- Inode table: `inode.py` class, dynamic allocation. ✔
- Directories: hierarchical nested dicts, `mkdir`, `cd`, `ls`. ✔
- Free-space bitmap: `bitmap.py` with allocate/free. ✔
- File data blocks: `data_blocks` list; multi-block files (chunked by block_size). ✔
- File ops: `create`, `read`, `write`, `rm` (delete). ✔
- Persistence (save/load): implemented via JSON export (optional). ✔

## How to run (local)
1. Install requirements:
   ```bash
   pip install -r requirements.txt
