# Day 5 — Linux Users and Groups

## Topics Covered

- Understanding Linux user accounts
- Understanding groups
- Difference between a normal user and root
- Basic user and group information commands
- How users, groups, and file permissions work together

## Commands Practised

### 1. `whoami`
Displays the username of the currently logged-in user.

```bash
whoami
```

### 2. `id`
Displays the current user's UID, GID, and group memberships.

```bash
id
```

### 3. `groups`
Displays the groups to which the current user belongs.

```bash
groups
```

## Important Concepts

**User:** An account used to access a Linux system.

**Group:** A collection of users that can share permissions to access files and resources.

**Root:** The Linux superuser with extensive administrative privileges.

**Permissions:** Rules that determine whether users can read, write, or execute files.

## How Users, Groups, and Permissions Work Together

Linux uses users, groups, and permissions to control access to files and directories.

For example, a file can have an owner and a group. Its permissions determine what the owner, group members, and other users are allowed to do.

## Key Takeaways

- `whoami` identifies the current user.
- `id` displays user and group IDs.
- `groups` displays group memberships.
- Root has extensive administrative privileges.
- Groups help manage access for multiple users.
- File permissions help protect system resources.

## Practice Environment

Browser-based Linux terminal: WebTerm

https://webterm.app/en/free-play

## Next Steps

- Revise Linux file permissions.
- Learn about file ownership.
- Understand the difference between `chmod` and `chown`.
- Continue practising Linux commands.
