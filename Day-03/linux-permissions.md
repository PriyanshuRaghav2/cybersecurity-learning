# Day 3 – Linux Permissions

Topics Learned

* Linux file permissions
* Read (r)
* Write (w)
* Execute (x)
* User / Owner
* Group
* Others
* ls -l
* chmod
* chown
* chgrp
* SUID
* SGID

Permission Basics

r = Read
w = Write
x = Execute


Linux permissions are divided into:

User
Group
Others


Check Permissions

ls -l


Example:

-rwxr-xr--

Owner  → rwx
Group  → r-x
Others → r--


chmod

Used to change file permissions.

chmod u+x script.sh
chmod g+w file.txt
chmod o-r file.txt

Numeric Permissions

r = 4
w = 2
x = 1


Common permissions:


600 = rw-------
644 = rw-r--r--
700 = rwx------
755 = rwxr-xr-x


Examples:

chmod 600 private.txt
chmod 644 file.txt
chmod 755 script.sh


Ownership


chown username file.txt
chgrp groupname file.txt


SUID

SUID allows an executable to run with the privileges of its file owner.

Example:

-rwsr-xr-x

SGID

chmod g+s file

Users and programs should have only the permissions they need.

Incorrect permissions can lead to unauthorized access and security vulnerabilities.

Commands Practiced

ls -l
chmod
chown
chgrp


