# Bandit 1-2
### Goal
Log in using SSH. Find the password for the next level.

### Info
- Host to connect to: bandit.labs.overthewire.org
- Port: 2220
- Current username: bandit1
- Current password: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
- bandit2 password is stored in a file called " **-** " 
- " **-** " is in the home directory

### Fundamentals
- `cat` : Shows the contents of a file right in the terminal.
- `ls -a` : Lists all the files in the current folder, including hidden files.
- " `./` " : Means "**in this directory**" (i.e. the current working directory)

### Solution
Note: Switched to [Git Bash](https://gitforwindows.org/) instead of PuTTY
- type `ssh bandit1@bandit.labs.overthewire.org -p 2220`
	- I want to securely access a user's (`bandit1`) account, on a certain server (`bandit.labs.overthewire.org`) on a certain port (`-p 2220`)
- type `cat ./-` or `cat /home/bandit1/-`

<img width="221" alt="OverTheWire - Bandit 2-1" src="https://github.com/user-attachments/assets/84cc70fc-a329-4ad6-9563-7445223d9cb9" />

- Password to log into bandit2 user: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx

### Helpful Stuff
- [Why we use ./ (dot slash) to run Linux scripts?](https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/Why-must-you-use-to-run-your-Ubuntu-scripts-The-meaning-of-Linuxs-dot-slash-explained)
- [How to create, open, find, remove dashed -file_name in Linux](https://medium.com/@.Qubit/how-to-create-open-find-remove-dashed-filename-in-linux-27ee297d1740)
- [Advanced Bash-Scripting Guide: Chapter 3 - Special Characters](https://linux.die.net/abs-guide/special-chars.html)
