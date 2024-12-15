```bash
# First N lines of a file
head -n N <file>

# Last N lines of file
tail -n N <file>

# display file contents
cat <file> <file>

# View contents of a file 1 page/line at a time
# press enter to continue, space to view the next page, b to go back, q to quit
less -N <file>

# Search for a string in a file (case sensitive)
grep "String" <file> 

# recursively search all files n a directory
grep -r "String" <dir>

# list files with permissions
ls -l

# list all (including hidden)
ls -a

# Permissions:
# r = read
# w = write
# x = execute
# d = directory
# r = regular file
drwx------ # admin/user can read write and execute, groups and others have no permissions to a directory

d---rwx--- # group has all permissions, admin/user and others have none.

d------rwx # only others have permissions.

# change permissions (-R recursively)

chmod -R u=rwx,g=rwx,o=rwx

# Remove/add the ability to execute
chmod -x <file>
chmod +x <file>

# sudo (super user do) needed when you don't own the file.
# chown - change owner

sudo chown -R <new owner> <dir>
```
