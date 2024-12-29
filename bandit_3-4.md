# Bandit 3-4
### Goal
Log in using SSH. Find the password for the next level.

### Info
- Current username: bandit3
- Current password: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
- bandit4 password is stored in a **hidden file**
- hidden file is in the **inhere** directory

### Fundamentals
- `ls -a` : to list ALL the files in the current folder, including **hidden files**.
- `pwd` : to check the current directory, and the full path to get there
- `cd` : to **change directory**. By default, when you log into your Linux system, the current directory is the home directory,
  - `cd [directory_name]` : move to a subdirectory **within the CURRENT directory**
  - <img width="202" alt="OverTheWire - Bandit 4-1" src="https://github.com/user-attachments/assets/c36e22d3-20c3-4648-adba-ce26e863c8b8" />
  - `cd /` : move to the root directory. The root directory is **the first directory** in the filesystem hierarchy
  - <img width="244" alt="OverTheWire - Bandit 4-2" src="https://github.com/user-attachments/assets/8f31dd48-f856-438b-b0e5-b7ff56a06ff9" />
  - `cd ..` : takes me to the parent directory of the current directory
  - <img width="377" alt="image" src="https://github.com/user-attachments/assets/d9a1bdef-38a8-4272-9a6b-d7824e25a778" />
  - `cd .` : refers to the current directory
  - `cd -` : to quickly switch between the current directory and the directory I was in before.
  - <img width="503" alt="image" src="https://github.com/user-attachments/assets/29928742-60fd-45cb-8084-27ba65c37057" />
  - `cd ~` : takes me back to the home ("`~`") directory.
    - So `cd ~/Downloads` would take me to the `Downloads` folder in my home directory.
    - `cd ~username` takes me to another user's home directory
	- `cd [directory] && ls` : adds the `ls` command.
  - `cd dir_1/dir_2/dir_3` : move inside a directory from a directory.
  - <img width="544" alt="image" src="https://github.com/user-attachments/assets/caee2752-a48d-40c5-bdaf-126c56d5664b" />
  - `cd 'Dir name with space'` or `cd Dir\ name\ with\ space` for directories with spaces.

### Solution
<img width="317" alt="OverTheWire - Bandit 4" src="https://github.com/user-attachments/assets/8c257356-6a13-4cb1-b800-d1b331b594a4" />

- Password for bandit4: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
  
### Helpful Stuff
- [How to Change the Directory in Linux | cd Command](https://www.geeksforgeeks.org/cd-command-in-linux-with-examples/)
- [cd Command: How to Change Directory in Linux](https://phoenixnap.com/kb/linux-cd-command)
