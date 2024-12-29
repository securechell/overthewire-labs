# Bandit 2-3
### Goal
Log in using SSH. Find password for next level.

### Info
- Current username: bandit2
- Current password: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx
- bandit3 password is stored in a file called **spaces in this filename** 
- **spaces in this filename** is in the home directory

### Fundamentals
- Linux files/folders/directories don't usually have spaces in the name. `-` (dash) or `_` (underscore) is used instead.
- The `spaces in this filename` file would look like 4 separate documents: `spaces`, `in`, `this`, and `filename`. So `cat spaces in this filename` wouldn't make sense:

<img width="353" alt="OverTheWire - Bandit 3-1" src="https://github.com/user-attachments/assets/d48a7e11-2558-428f-b6b5-620b00f66f77" />

- To overcome this either:
	- put the file name in **quotes** (single or double): `cat "spaces in this filename"`
	- or put a backslash **in front of every space** in the filename (to "escape" the space): `cat spaces\ in\ this\ filename`

### Solution
- With quotes:
<img width="386" alt="OverTheWire - Bandit 3" src="https://github.com/user-attachments/assets/27de4449-f5e8-4abb-8fe6-eb2d31219dfe" />

- Without quotes:
<img width="317" alt="OverTheWire - Bandit 3-2" src="https://github.com/user-attachments/assets/1dae1d5f-4ddf-4b08-9c32-d3d391ed9fcb" />

- Password for bandit3 user: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

### Helpful Stuff
- [How to Tackle Filenames With Spaces in Linux](https://linuxhandbook.com/filename-spaces-linux/)
