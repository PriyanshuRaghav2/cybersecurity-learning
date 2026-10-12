# Day 4 — Linux File Permissions and User Management

## 1. Linux File Permissions

Linux permissions control what users can do with files and directories.

- **Read (r):** Allows reading a file.
- **Write (w):** Allows modifying a file.
- **Execute (x):** Allows executing a program or accessing a directory.

## 2. Permission Categories

- **User (u):** The file owner. 
- **Group (g):** Users who belong to the file's group. 
- **Others (o):** All other users.

Example:

`-rw-r--r--`

The owner can read and write, while the group and others can only read.

## 3. chmod Command

The `chmod` command changes file permissions.

Examples:

- `chmod 600 notebook.txt` — owner can read and write.
- `chmod 644 notebook.txt` — owner can read and write; group and others can read.
- `chmod 700 notebook.txt` — owner has read, write, and execute permissions.

## 4. Viewing Permissions

The `ls -l` command displays file details, including permissions.

Example:

`ls -l notebook.txt`

## 5. Basic User Management

- `whoami` — displays the current username.
- `id` — displays user ID and group information.
- `groups` — displays the groups the current user belongs to.
- **Root:** The Linux superuser with extensive administrative privileges.

## 6. Commands Practised

- `mkdir` — creates a directory.
- `cd` — changes the current directory.
- `touch` — creates an empty file if it does not exist.
- `ls -l` — displays file permissions.
- `chmod` — changes file permissions.
- `whoami`, `id`, and `groups` — show user and group information.

## 7. Key Learning

Linux file permissions help control access to files and directories. User accounts and groups help organise access and separate privileges.

## 8. Next Steps

Revise permission numbers and practise reading the output of `ls -l` before moving on to advanced permissions.
