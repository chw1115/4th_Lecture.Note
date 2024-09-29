# 4th_Lecture.Note
Assignment of Open Source SW


## CLI vs GUI
### CLI
- Have to momorize command
- Fast
- Developer oriented

### GUI
- Easy to use
- Slow
- User-friendly for general users
----

## Shell Command

#### pwd
Display the current working directory.

### cd
Change the directory.
- /: Root directory.
- .:current directory.
- ..:upper-level directory.
- ~:home of current user.
- /[directory name]:absolute path

### ls
list files and directories.
- -l: Show detailed information(long format).
- -lh: Same as above, but size in units.
- /bin: List the files in the **/bin** directory ( or any other directory we care to specify).
- -l/etc/bin: List the files in the **/bin** directory and the **/etc** directory in long format.
- -la..: List all files in the parent of the woring directory in long format


> #### Long Format
> File Permissions | Owner | Group |   Size(in bytes) | Modification Time | File Name
> #### TIP
> press **Tab** key to autocompletion
> press up arrow key "//" to copy previous commands.

### clear
Clear terminal screen.

---
## Manipulation

### cp
copy files and directories
- cp file1 file2: Copies the contents of file1 into file2. If file2 does not exists, it is created; **otherwise, file2 is silently overwiritten with the contents of file1**.
- cp -i file1 file2: Like as above, However, since "-i"(interactive) option is specified, if files 2 exist, the user is prompted before it is overwritten with the contents of file 1. 
- cp file1 dir1: Copies file1(into a file named *file1*)into directory dir1.
- cp -r dir1 dir2: Recursively copies directory dir1 to dir2 if directory dir2 does not exist, it is created. Otherwise, it creates a a directory named dir1 within directory dir2.
 
### mv
move files and directories or rename them.
- mv file1 file2: Rename file1 to file2. If file2 exists, the content of file2 
- mv -i file1 file2: Like as above, However since the "-i"(interactive) option is specified, if file2 exist, the user is prompted bofore it is overwritten with the contents of file1.
- mv file1 file2 dir1: Moves file1 and file2 to directory dir1. If dir1 does not exist, **mv** will exit with an error.
- mv dir1 dir2: if dir2 does not exist, Rename dir1 to dir2. If dir2 exists, the directory dir1 is moved within directory dir2.

### rm 
delete files and directories.
- rm file1 file2: delete file1 and file2.
- rm -i file1 file2: Because of "i", the user is prompted before each file is deleted.
- rm -r dir1 dir2: Directories dir1 and dir2 are deleted along with all of their contents.

### mkr
make a new directory.

### Wildcards
 - *: Matches all filenames.
 - g*: Matches all filenames starting with 'g'.
 - b*.txt: Matches all .txt files starting with 'b'.
 - Data???: Matches filenames like Data123, but not Data12

## Help

### Help
Display the options for help 

### Man
Display information about command.

## Exit

### Exit 
Exit the terminal

