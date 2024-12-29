# Bandit 5-6
### Goal
Log in using SSH. Find password for next level.

### Info
- Current username: bandit5
- Current password: 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
- bandit6 password is:
	- stored in a file in the **inhere** directory
	- human-readable
	- 1033 bytes in size
	- not executable

### Fundamentals
- `file` : examines content and gives info on the type of file
- `find` : allows you to search for files and directories based on various criteria such as name, ownership, size, type, and modification date. A v.powerful command!
- `find` syntax is: `find [directory to search] [options] [expression]`
	- `[directory to search]` : Location where you want to start the search. Use `.` to represent the current directory. If the `[directory to search]` isn't specified, it searches the current directory and its sub-directories by default.
	- `[options]` : Specifies the **type** of search, e.g. by name, by type, by time modified etc.
	- `[expression]` : Specifies the search criteria. e.g., if you wanted to find a file by its name, `[expression]` would be the file name.
- some `find` possibilities:
  - `-name`: look for a file or directory by name.
  - `find . -name mystuff` will search for files *and* directories with the name `mystuff` (in the current directory "`.`")
    <img width="357" alt="OverTheWire - Bandit 5-6-4" src="https://github.com/user-attachments/assets/500b2832-ddfa-45af-b63f-ebca6a3c5aa1" />
  - add `-type f` to only look for *files*, e.g. `find . -type f -name mystuff`
  - <img width="385" alt="OverTheWire - Bandit 5-6-5" src="https://github.com/user-attachments/assets/26e1712b-7560-45c4-a6c3-e18d01d523fa" />
  - add `-type d` to only search for *directories*
  - <img width="323" alt="OverTheWire - Bandit 5-6-6" src="https://github.com/user-attachments/assets/c6376ff8-bce7-446a-8efd-8b4a3ac63763" />

- `-size`: search for a file based on its size. This only works with files, not directories.
  - `find . -size 50k` will show files that are exactly 50 KB
  - `find . -size +1G` will look for files bigger than 1 GB
  - `find . -size -20c` will show files smaller than 20 bytes
  - `find . -size +100M -size -2G` will show files larger than 100 MB, but smaller than 2 GB


### Solution
<img width="410" alt="OverTheWire - Bandit 5-6" src="https://github.com/user-attachments/assets/cfca253c-8f4b-41c0-b0f1-b7ae0dca991a" />

- `find . -size 1033c`
<img width="259" alt="OverTheWire - Bandit 5-6-2" src="https://github.com/user-attachments/assets/02ba6919-4529-42ba-9404-a5fd1a6798bd" />

- So password must be in `./maybehere07/.file2`
<img width="323" alt="OverTheWire - Bandit 5-6-3" src="https://github.com/user-attachments/assets/88fbaf7a-5422-4f55-9a82-f55d6f301ca4" />

- Password for bandit6 : HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
### Helpful Stuff
- [find Command Examples](https://linuxhandbook.com/find-command-examples/)
