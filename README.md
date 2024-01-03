This project entails creating a C-language program called "tarsau," akin to archiving tools like tar, rar, or zip, but without compression. Here's a summary:

#Program Overview:

## tarsau –b: 
- Combines text files (ASCII, 1 byte per character) into a single text file.
- Limits: Total input file size ≤ 200 MB, number of input files ≤ 32.
- Handles incompatible formats, exiting cleanly with a message.
- Command format: tarsau –b file1 file2 ... –o output.sau

## tarsau –a: 
- Extracts files from the archive to a specified directory.
- Command format: tarsau –a archive.sau directory
- Checks for appropriate archive file and directory names.
- Creates directory if non-existent and preserves file permissions.

#Archive File Format (.sau):

- Consists of two sections: Organization info and Archived files.
- Organization section: Holds metadata (file name, permissions, size).
- Archived files: Stored in ASCII without delimiters, with the last character indicating EOF.


#Steps Involved:

- Design and implement "tarsau" program in C.
- Ensure functionality to combine text files without compression.
- Validate input file formats and handle errors gracefully.
- Create the archive file in the specified format.
- Implement extraction of files from the archive with correct permissions.
-
-

-The project requires careful handling of file operations, error checking, and adherence to the specified file format. Collaboration and version control using GitHub are also integral to the development process.
