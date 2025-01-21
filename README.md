Recover

Project Description

Recover is a program developed as part of the CS50 course. This program performs file recovery by scanning a forensic image for JPEG files and restoring them. It demonstrates fundamental programming concepts such as file I/O, data recovery, and memory management in C.

This project simulates a real-world scenario of recovering data from corrupted or deleted storage devices, making it an excellent learning experience in forensic computing and low-level programming.

Features

Identifies JPEG headers in a forensic image.

Recovers JPEG files by writing them to separate files.

Handles varying numbers of JPEG files and ensures correct restoration.

Implements efficient file I/O and memory management techniques.

How It Works

The program reads a forensic image file byte by byte.

It detects the beginning of a JPEG file by identifying JPEG headers (starting bytes 0xff 0xd8 0xff 0xe0 or 0xff 0xd8 0xff 0xe1).

Once a JPEG header is found, the program writes the file to disk and continues scanning for the next JPEG.

The process continues until the entire forensic image is processed.

Getting Started

Prerequisites

GCC compiler or any C compiler.

Basic knowledge of C programming.

Installation

Clone the repository:

git clone https://github.com/your-username/recover.git

Navigate to the project directory:

cd recover

Compile the program:

make recover

Usage

Run the program with the following command:

./recover forensic_image.raw

Replace forensic_image.raw with the path to the forensic image file you want to recover JPEGs from.

Output

Recovered JPEG files are saved in the current working directory with names like 000.jpg, 001.jpg, and so on.

Example

$ ./recover card.raw
Recovered 50 JPEG files.

After running the command, you will find files named 000.jpg, 001.jpg, ... up to 049.jpg in the working directory.

File Structure

recover.c: Main program file containing the implementation.

Makefile: For compiling the program.

forensic_image.raw: Example forensic image (optional, for testing purposes).

Learnings

This project helped in understanding:

How to work with binary files in C.

Data recovery techniques by analyzing file signatures.

Memory management and file handling.

Contributions

Contributions are welcome! Feel free to fork the repository and submit a pull request.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments

This project is part of the CS50 course by Harvard University. Thanks to the course staff and community for their guidance and support.
