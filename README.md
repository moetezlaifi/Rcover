# Recover

## Project Description

Recover is a program developed as part of the CS50 course. This program performs file recovery by scanning a forensic image for JPEG files and restoring them. It demonstrates fundamental programming concepts such as file I/O, data recovery, and memory management in C.

This project simulates a real-world scenario of recovering data from corrupted or deleted storage devices, making it an excellent learning experience in forensic computing and low-level programming.

## Features

- Identifies JPEG headers in a forensic image.
- Recovers JPEG files by writing them to separate files.
- Handles varying numbers of JPEG files and ensures correct restoration.
- Implements efficient file I/O and memory management techniques.

## How It Works

1. The program reads a forensic image file byte by byte.
2. It detects the beginning of a JPEG file by identifying JPEG headers:
   - Starting bytes: `0xff 0xd8 0xff 0xe0` or `0xff 0xd8 0xff 0xe1`.
3. Once a JPEG header is found, the program writes the file to disk and continues scanning for the next JPEG.
4. The process continues until the entire forensic image is processed.

##Learnings
This project helped in understanding:

- How to work with binary files in C.
- Data recovery techniques by analyzing file signatures.
- Memory management and file handling.

##Contributions
Contributions are welcome! Feel free to fork the repository and submit a pull request.

##License
This project is licensed under the MIT License.

##Acknowledgments
This project is part of the CS50 course by Harvard University. Thanks to the course staff and community for their guidance and support.
