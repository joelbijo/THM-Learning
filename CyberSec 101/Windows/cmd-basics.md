# Basic CMD

1. **ipconfig** -> Show the network address settings for the computer.
2. **/?** -> To retrieve the help manual for a command.
3. **netstat** -> Display protocol statistics and current TCP/IP network connections.

- For netstat, to display the manual, use command: `netstat help`.

4. **ssh** -> Secure Shell Command. It is used to securely connect to a remote computer or server over an unsecured network.

- eg: ssh user@10.48.124.201

5. **systeminfo** -> To find the build details of the system, like OS version, memory available etc.

## Network Troubleshooting

1. **nslookup** -> It looks up a host or domain and returns its IP address.
2. **tracert** -> Traces the network route traversed to reach the target.
3. **ping** -> It is simplest way of checking whether an ip or website is reachable and it can reach the source system as well.
4. **netstat** -> Displays current network connections and listening ports.

- netstat -abon -> Displays established connections(-a), programs associated(-b), process id(-o), numerical form for addresses and port numbers(-n).

_The service listening on port 135 is the Microsoft RPC Endpoint Mapper (also known as Remote Procedure Call or MSRPC)._

5. **dir**

- **dir /a** - Displays hidden and system files as well.
- **dir /s** - Displays files in the current directory and all subdirectories.

6. **tree** To visually represent the child directories and subdirectories.

**The wildcard character _ to refer to multiple files. For example, copy _.md C:\Markdown will copy all files with the extension md to the directory C:\Markdown.**

7. **del or erase** To delete a file.

8. **tasklist** To list the running processes.
   `/FI` is used to set the filter
   eg: `tasklist /FI "imagename eq sshd.exe"`

9. **taskkill** Terminate any task if PID known.
   Eg: `taskkill /PID target_pid`
