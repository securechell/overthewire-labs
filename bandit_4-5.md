# Bandit 4-5
### Goal
Log in using SSH. Find password for next level.

### Info
- Current username: bandit4
- Current password: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
- bandit5 password is stored in a file in the **inhere** directory
- File is the only human-readable file in the directory

### Fundamentals
- `file` : gives info on the type of file. It identifies file types by examining their **content** rather than their file extensions. The file type can be displayed in a **human-readable** format (e.g., ASCII, Unicode) or as a **MIME type**.
- To open a file that starts with a dash ( `-` ) use: `< -` or `./-`
	- e.g. `cat < -file_name` or `cat ./-file_name`
- To apply a command on all the files in the current directory, use the wildcard symbol (` * `). This can stand for any character.
	- e.g. `file*`, selects everything that starts with "file", such as ‘file00’, ‘file’, ‘fileAA’, 'file_1', etc.

### Solution
- `cd` to `inhere`:
- ![OverTheWire - Bandit 5-1](https://github.com/user-attachments/assets/9ecc6cba-8ba4-4f17-bade-353cdd352513)
- `file ./-file*` :
- <img width="307" alt="OverTheWire - Bandit 5-2" src="https://github.com/user-attachments/assets/d39feb0a-8da0-4376-8d58-6f581735b43b" />
- Password for bandit5 : 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
### Helpful Stuff
- [file command in Linux with examples](https://www.geeksforgeeks.org/file-command-in-linux-with-examples/)
