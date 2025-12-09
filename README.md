# rendező — simple folder organizer

A small Python script that opens a folder picker and moves files from the selected directory into subfolders based on file extensions.

This repository contains a single script (rendező.py) that provides a quick way to organize the files in a directory into categorized folders.

Features
- Opens a folder selection dialog (tkinter) to choose the target directory.
- Moves only files in the chosen directory (top-level) into subfolders based on extension.
- Creates target subfolders if they don't exist.
- Uses a configurable mapping (see "Customization").

Quick start

Prerequisites
- Python 3
- tkinter (usually included with standard Python installations)

Run

1. From a terminal: python rendező.py  (or python3 rendező.py)
2. A dialog will open to select the directory to organize.
3. The script moves files and prints "kész az elrendezés" when finished, then waits for Enter (input()).

Behavior details
- Only the files directly inside the selected folder are processed. Files in nested subdirectories are ignored.
- The script determines file extension by splitting the filename on the last dot (filename.split('.')[-1].lower()). Files without a dot will be treated as having the entire filename as the "extension" and therefore usually won't match any mapping.
- If a destination filename already exists, behavior depends on the OS and shutil.move: name collisions can raise errors or overwrite; test on a small folder first.

Default extension → folder mapping
(The mapping is defined in the anyaaa dictionary in rendező.py)
- pdf: PDF-ek
- png, jpg, jpeg, gif: Képek
- doc, docx, txt: Dokumentumok
- csv, xlsx: Adatok
- zip, rar: Tömörítvények
- exe: Programok
- mp3, wav: Zenék
- mp4, avi, flv, wmv: Videók
- c: C-programok
- py: Python-programok
- html: html-weboldalak

Customization
- Edit the anyaaa dictionary in rendező.py to add, remove or change extension mappings.
- You can localize the folder names or add other extensions as needed.

Notes
- The script prints messages and uses Hungarian strings (e.g., "kész az elrendezés"). Edit the source if you prefer English messages.
- Be cautious when running on folders with many files or important data. Test on a sample directory first.

Reference
- Main script: rendező.py
