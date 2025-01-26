# Automatic File Sorter

## Description
The **Automatic File Sorter** is a Python script that helps you organize files in a specified directory by automatically sorting them into categorized folders based on their file types. This script is particularly useful for keeping your workspace tidy and managing large volumes of files efficiently.

## Features
- Automatically identifies file types (`.xlsx`, `.jpg`, `.txt`) in a directory.
- Creates categorized folders (`xlsx files`, `image files`, `text files`) if they don't already exist.
- Moves files into their respective folders based on file extensions.
- Ensures no duplicate files are moved.

## How It Works
1. Specify the target directory path in the script.
2. The script creates subfolders (`xlsx files`, `image files`, `text files`) within the directory if they are missing.
3. Files in the target directory are scanned and moved to their respective folders based on their extensions.
4. The script skips already-sorted files to avoid duplication.

## Requirements
- **Python 3.x**
- Libraries: `os`, `shutil`

## Usage
1.Clone the repository:
   ```bash
   git clone https://github.com/yash-khobragade/automatic-file-sorter.git
```
2.Navigate to the project folder:
```bash
    cd automatic-file-sorter
```

3.Edit the path variable in the script to match the directory you want to organize.

4.Run the script:
```bash
    python file_sorter.py
```

Example

If the target folder contains:

report.xlsx                                                                                                                                                                                                    
photo.jpg                                                                                                                                                                                                    
notes.txt

After running the script, the folder structure will look like:
```
New folder/
│
├── xlsx files/
│   └── report.xlsx
├── image files/
│   └── photo.jpg
└── text files/
    └── notes.txt
```



