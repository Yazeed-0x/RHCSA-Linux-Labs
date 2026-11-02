LAB 01 — Linux File Permissions

##Objective
Learn how to create files and directories and manage file permissions in Red Hat Enterprise Linux.

##Environment
- OS: Red Hat Enterprise Linux
- Virtualization: VirtualBox
- Network: Isolated

##Tasks Completed
- Created directories using `mkdir`.
- Created files using `touch`.
- Wrote text using `echo`.
- Modified file permissions using `chmod`.
- Verified permissions using `ls -l` and `stat`.

##Commands Used

```bash
mkdir -p ~/linux-labs/lab01/reports
mkdir -p ~/linux-labs/lab01/support

chmod 600 ~/linux-labs/lab01/reports/sales.txt
chmod 640 ~/linux-labs/lab01/support/tickets.txt

stat -c "%a %n" ~/linux-labs/lab01/reports/sales.txt
stat -c "%a %n" ~/linux-labs/lab01/support/tickets.txt
```

##What I Learned
I learned how Linux permissions work for the owner, group, and others.

- `600`: Owner can read and write.
- `640`: Owner can read and write; group can read.
- `chmod`: Changes file permissions.
- `stat`: Displays detailed file information.

##Lab Status
Completed

Evidence
Screenshots of the verification results will be added.
