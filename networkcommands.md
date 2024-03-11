### ifconfig:
Display information about network interfaces, including IP addresses, MAC addresses, and network statistics.
### ip:
A versatile tool for configuring network interfaces, routing tables, and tunnels.
- ex: ip addr,ip route
### netstat:
Display information about network connections, routing tables, interface statistics, masquerade connections, etc.
- ex: netstat -an
### ping:
Check network connectivity to a specific host.
- ex: ping google.com
### traceroute:
Trace the route that packets take to reach a destination.
- ex:traceroute google.com
### nslookup:
Trace the route that packets take to reach a destination.
- ex:nslookup google.com
### nslookup or dig:
Perform DNS lookups to resolve domain names to IP addresses.
### curl or wget:
Fetch data from a specified URL, useful for testing connectivity.
- ex: curl http://example.com
### ss:
Display socket statistics, including listening and established connections.
- ex:ss -tulpn
### iptables:
View and manipulate IP packet filter rules.
- ex:iptables -L
### route:
Display or manipulate the IP routing table.
- ex:route -n
### ethtool:
Display or change ethernet card settings, such as speed, duplex, and link status.
- ex:ethtool eth0
### arp:
Display or manipulate the ARP cache.
- ex:arp -a
### sshd:
Check the status of the SSH server, useful for debugging connectivity issues.
- ex:ps aux | grep sshd
### resolv.conf:
Check the DNS configuration by examining the contents of the /etc/resolv.conf file.
- ex:cat /etc/resolv.conf

## 𝗬𝗼𝘂 𝗠𝗨𝗦𝗧 𝗟𝗲𝗮𝗿𝗻 𝘁𝗵𝗲 𝗟𝗶𝗻𝘂𝘅 𝗳𝗶𝗹𝗲 𝘀𝘆𝘀𝘁𝗲𝗺

Linux's file system is tree-like. The base is "/", with everything else branching off.

Core Directories:

/bin 🛠: Essential binaries, e.g., bash, ls, grep.
/boot 🚀: Boot items like kernel & bootloader.
/dev 🔌: Device files for connected hardware.
/etc 📜: System configuration files.
/home 🏠: User home directories.
/lib 📚: Shared libraries for programs.
/media 💿: Mounts for removable media.
/mnt 🧲: Temporary mounts.
/opt 📦: Optional software.
/proc 📊: System, process, memory info.
/root 👑: Root user's home.
/sbin 🔧: System admin tools, e.g., init.
/srv 🌐: Data for services.
/tmp 🌡: Temporary files.
/usr 🖥: User software.
/var 🔄: Variable data, logs, temp files.

Linux Commands:

cd 🚶: Navigate.
ls 📋: List contents.
mkdir 📁: Create folder.
rmdir 🗑: Delete folder.
cp 📤: Copy.
mv 🚚: Move.
rm ❌: Delete.

⚠ Note: Directories like /bin are crucial. Don't modify!


## 𝐇𝐞𝐫𝐞 𝐚𝐫𝐞 𝐬𝐨𝐦𝐞 𝐜𝐨𝐦𝐦𝐨𝐧 𝐞𝐫𝐫𝐨𝐫𝐬 𝐢𝐧 𝐋𝐢𝐧𝐮𝐱 𝐚𝐧𝐝 𝐭𝐡𝐞𝐢𝐫 𝐬𝐨𝐥𝐮𝐭𝐢𝐨𝐧𝐬:

1. 🚫 𝐂𝐨𝐦𝐦𝐚𝐧𝐝 𝐍𝐨𝐭 𝐅𝐨𝐮𝐧𝐝 🚫
𝐄𝐫𝐫𝐨𝐫: 🚫When you try to run a command, and Linux responds with "𝐜𝐨𝐦𝐦𝐚𝐧𝐝 𝐧𝐨𝐭 𝐟𝐨𝐮𝐧𝐝."
𝐒𝐨𝐥𝐮𝐭𝐢𝐨𝐧: 🛠 Ensure that the command is spelled correctly and that the program is installed. Use the 𝐰𝐡𝐢𝐜𝐡 or 𝐰𝐡𝐞𝐫𝐞𝐢𝐬 command to locate the executable and check your system's PATH variable.

2. 𝐏𝐞𝐫𝐦𝐢𝐬𝐬𝐢𝐨𝐧 𝐃𝐞𝐧𝐢𝐞𝐝:
𝐄𝐫𝐫𝐨𝐫:  🔒 You don't have the necessary permissions to access or modify a file or directory.
𝐒𝐨𝐥𝐮𝐭𝐢𝐨𝐧: 🔓Use the 𝐜𝐡𝐦𝐨𝐝 command to change permissions, and 𝐜𝐡𝐨𝐰𝐧 to change ownership. You may need to use 𝐬𝐮𝐝𝐨 to gain superuser privileges.

3. 𝐍𝐨 𝐒𝐩𝐚𝐜𝐞 𝐋𝐞𝐟𝐭 𝐨𝐧 𝐃𝐞𝐯𝐢𝐜𝐞:
𝐄𝐫𝐫𝐨𝐫: 💾  This error occurs when your disk is full.
𝐒𝐨𝐥𝐮𝐭𝐢𝐨𝐧:  🗑 You need to free up space by deleting unnecessary files or moving them to another disk. You can use the 𝐝𝐟 & 𝐝𝐮 commands to identify space hogs.

4. 𝐃𝐞𝐩𝐞𝐧𝐝𝐞𝐧𝐜𝐲 𝐈𝐬𝐬𝐮𝐞𝐬:
𝐄𝐫𝐫𝐨𝐫: A program won't run because it's missing dependencies.
𝐒𝐨𝐥𝐮𝐭𝐢𝐨𝐧: Use your package manager (e.g., apt, yum, dnf) to install the missing libraries or packages.

5. 𝐍𝐞𝐭𝐰𝐨𝐫𝐤 𝐈𝐬𝐬𝐮𝐞𝐬:
𝐄𝐫𝐫𝐨𝐫: Network connectivity problems, such as no internet connection.
𝐒𝐨𝐥𝐮𝐭𝐢𝐨𝐧: Check your network settings, restart the network service (𝐬𝐲𝐬𝐭𝐞𝐦𝐜𝐭𝐥 𝐫𝐞𝐬𝐭𝐚𝐫𝐭 𝐍𝐞𝐭𝐰𝐨𝐫𝐤𝐌𝐚𝐧𝐚𝐠𝐞𝐫), or troubleshoot using tools like 𝐩𝐢𝐧𝐠, 𝐢𝐟𝐜𝐨𝐧𝐟𝐢𝐠, 𝐚𝐧𝐝 𝐧𝐦𝐜𝐥𝐢.

6. 𝐅𝐢𝐥𝐞𝐬𝐲𝐬𝐭𝐞𝐦 𝐂𝐨𝐫𝐫𝐮𝐩𝐭𝐢𝐨𝐧:
𝐄𝐫𝐫𝐨𝐫: The filesystem reports errors, or you can't access files.
𝐒𝐨𝐥𝐮𝐭𝐢𝐨𝐧: Use filesystem repair tools like 𝐟𝐬𝐜𝐤 to fix errors.

7. 𝐒𝐭𝐮𝐜𝐤 𝐏𝐫𝐨𝐜𝐞𝐬𝐬:
𝐄𝐫𝐫𝐨𝐫: A process is stuck and not responding.
𝐒𝐨𝐥𝐮𝐭𝐢𝐨𝐧: Use the 𝐤𝐢𝐥𝐥 command to terminate the process.

8. 𝐒𝐥𝐨𝐰 𝐒𝐲𝐬𝐭𝐞𝐦:
𝐄𝐫𝐫𝐨𝐫: Your system is slow and unresponsive.
𝐒𝐨𝐥𝐮𝐭𝐢𝐨𝐧: Identify resource-hungry processes with commands like 𝐭𝐨𝐩 𝐨𝐫 𝐡𝐭𝐨𝐩, and consider adding more 𝐑𝐀𝐌 or upgrading your 𝐡𝐚𝐫𝐝𝐰𝐚𝐫𝐞.

9. 𝐈𝐧𝐨𝐝𝐞 𝐄𝐱𝐡𝐚𝐮𝐬𝐭𝐞𝐝:
𝐄𝐫𝐫𝐨𝐫: When you run out of available 𝐢𝐧𝐨𝐝𝐞𝐬 on a file system.
𝐒𝐨𝐥𝐮𝐭𝐢𝐨𝐧: Delete unnecessary files and directories or reformat the partition with a larger 𝐢𝐧𝐨𝐝𝐞 count.

10. 𝐂𝐨𝐦𝐦𝐚𝐧𝐝 𝐒𝐲𝐧𝐭𝐚𝐱 𝐄𝐫𝐫𝐨𝐫𝐬:
𝐄𝐫𝐫𝐨𝐫: 🤔 You get errors related to the syntax of a command.
𝐒𝐨𝐥𝐮𝐭𝐢𝐨𝐧: Review the command's syntax, consult the manual pages (use 𝐦𝐚𝐧), or check online resources for the correct usage.

11. 𝐅𝐢𝐥𝐞 𝐍𝐨𝐭 𝐅𝐨𝐮𝐧𝐝:
𝐄𝐫𝐫𝐨𝐫:📁 File not found
𝐒𝐨𝐥𝐮𝐭𝐢𝐨𝐧:  🧐 Verify file location and name. Use the ls command to list files in a directory.

### ☄ Top Linux commands that are commonly used in DevOps: ♾

1. ls: List directory contents
2. cd: Change directory
3. pwd: Print working directory
4. mkdir: Create a directory
5. touch: Create a file
6. cp: Copy files and directories
7. mv: Move or rename files and directories
8. rm: Remove files and directories
9. find: Search for files and directories
10. grep: Search for patterns in files
11. cat: Concatenate and display files
12. less: View file contents page by page
13.head: Display the first lines of a file
14. tail: Display the last lines of a file
15. vi/vim: Text editor
16. nano: Text editor
17. tar: Archive and compress files
18. gzip: Compress files
19. gunzip: Decompress files
20. wget: Download files from the web
21. curl: Transfer data to or from a server
22. ssh: Secure shell remote login
23. scp: Securely copy files between hosts
24. chmod: Change file permissions
25. chown: Change file ownership
26. chgrp: Change group ownership
27. ps: Display running processes
28. top: Monitor system resources and processes
29. kill: Terminate processes
30. df: Display disk space usage
31. du: Estimate file and directory space usage
32. free: Display memory usage
33. uname: Print system information
34. ifconfig: Configure network interfaces
35. ping: Test network connectivity
36. netstat: Network statistics
37. iptables: Firewall administration
38. systemctl: Manage system services
39. journalctl: Query the system journal
40. crontab: Schedule cron jobs
41. useradd: Create a user account
42. passwd: Change user password
43. su: Switch user
44. sudo: Execute a command as another user
45. usermod: Modify user account
46. groupadd: Create a group
47. groupmod: Modify a group
48. id: Print user and group information
49. ssh-keygen: Generate SSH key pairs
50. rsync: Synchronize files and directories
51. diff: Compare files line by line
52. patch: Apply a patch to files
53. tar: Extract files from an archive
54. curl: Perform HTTP requests
55. nc: Netcat - networking utility
56. wget: Download files from the web
57. whois: Lookup domain registration details
58. dig: DNS lookup utility
59. sed: Stream editor for text manipulation
60. awk: Pattern scanning and processing language
61. sort: Sort lines in a text file
62. cut: Extract sections from lines of files
63. wc: Word, line, character, and byte count
64. tee: Redirect output to multiple files or commands
65. history: Command history
66. source: Execute commands from a file in the current shell
67. alias: Create command aliases
68. ln: Create links between files
69. uname: Print system information
70. lsof: List open files and processes
71. mkfs: Create a file system
72. mount: Mount a file system
73. umount: Unmount a file system
74. ssh-agent: Manage SSH keys in memory
75. grep: Search for patterns in files
76. tr: Translate characters
77. cut: Select portions of lines from files
78. paste: Merge lines of files
79. uniq: Report or omit repeated lines




