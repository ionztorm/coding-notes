# Terminal Commands

## Navigation

```bash
cd <dir> # change directory
cd .. # go up one directory
cd ~ # go to home directory
cd - # go to previous directory
cd / # go to root directory
cd . # current directory
```

## File Operations

```bash
touch <file> # create a file
rm <file> # remove a file
rm -r <dir> # remove a directory (r = recursive)
rm -f <file> # force remove a file
mv <file> <new file> # move a file
cp <file> <new file> # copy a file
```

## File Permissions

```bash
chmod u=rwx,g=rwx,o=rwx <file> # change permissions
chmod -R u=rwx,g=rwx,o=rwx <dir> # change permissions recursively
chmod -x <file> # remove the ability to execute
chmod +x <file> # add the ability to execute
sudo chown -R <new owner> <dir> # change owner
sudo chown -R <new owner>:<new group> <dir> # change owner and group
```

## File Viewing

```bash
head -n N <file> # first N lines of a file
tail -n N <file> # last N lines of a file
less -N <file> # view contents of a file 1 page/line at a time
more <file> # view contents of a file 1 page/line at a time
cat <file> <file> # display file contents
```

```

## File Searching
```bash
grep "String" <file> # search for a string in a file (case sensitive)
grep -r "String" <dir> # recursively search all files in a directory
grep -i "String" <file> # search for a string in a file (case insensitive)
find [path] [options] [expression] # find
find . -name <file> # find a file
find . -type f # find all files
find . -type d # find all directories
```

## File Listing

```bash
ls -l # list files with permissions
ls -a # list all files (including hidden)
ls -lh # list files with human readable sizes
ls -lt # list files by last modified time
ls -R # list files recursively
ls -d */ # list directories only
ls -F # list files with type indicators
ls -i # list files with inode numbers
```

## Programs exit codes

### Record the exit code of the last command in a file

```bash
./program.sh 2> error.log
```

## Process Management

```bash
ps # list processes
ps -ef # list all processes
ps aux # list all processes
kill <pid> # kill a process by process id
kill -9 <pid> # force kill a process by process id
```

# Variables

```bash
export VAR=value # set an environment variable
```

```
```
