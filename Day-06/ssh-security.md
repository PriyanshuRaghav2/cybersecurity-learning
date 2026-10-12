# Day 6 — SSH and Remote Access Security 

## 1. What is SSH? 

SSH stands for Secure Shell. It is a network protocol used to securely connect to and manage another computer over a network. SSH encrypts the communication between the client and server.

## 2. Important Concepts 

- **SSH Client:** The program used to connect to a remote computer.
- **SSH Server:** The service that accepts incoming SSH connections.
- **Default Port:** TCP port 22.
- **Password Authentication:** Uses an account password to log in.
- **SSH Key Authentication:** Uses a public and private key pair for authentication.

## 3. Linux Commands Practised 

### Check SSH Version 

```bash
ssh -V
```

Displays the installed SSH client version.

### Locate SSH

```bash
which ssh
```

Shows the path of the SSH executable.

### Check Listening TCP Ports

```bash
ss -tln
```

Displays TCP ports on which services are listening.

### Check Network Interfaces

```bash
ip addr
```

Displays network interfaces and their IP addresses.

### Generate an SSH Key Pair

```bash
ssh-keygen -t ed25519
```

Generates an SSH public and private key pair.

**Important:** Never share your private key or upload it to GitHub.

### Read SSH Server Configuration

```bash
less /etc/ssh/sshd_config
```

Displays the SSH server configuration file, if it exists.

## 4. SSH Client vs. SSH Server

- The client initiates a connection.
- The server accepts incoming connections and authenticates users.
- Installing an SSH client does not automatically enable an SSH server.
- SSH allows administrators to manage remote Linux systems securely.

## 5. Basic SSH Security Practices

1. Use strong passwords and protect private keys with a passphrase.
2. Keep Linux and OpenSSH updated.
3. Allow SSH access only to trusted users.
4. Avoid exposing SSH directly to the public internet unnecessarily.
5. Use key-based authentication where appropriate.
6. Never share private keys, passwords, or other sensitive information.

