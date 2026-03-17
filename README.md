#Linux-Basic-Assignment-Mahalakshmi
SECTION 1 – Write the purpose and an example usage for each command.
1.  pwd - Shows the current working directory (ex:/home/user/Desktop)
2.  ls - Lists files and folders in the current directory (ex:SQL  Java  README.md)
3.  cd - Changes the current directory (ex:/home/user/Desktop/maha-greens/SQL) 
4.  mkdir - Creates a new directory (ex:SQL  Java  README.md)
5.  rm -rf - Deletes a file or directory recursively and forcefully (ex:SQL  Java  README.md)
6.  ps -ef - Lists all running processes with full details (ex: UID   PID  PPID  C  STIME  TTY  TIME CMD)
7.  top - Displays real-time system processes and resource usage (ex:Shows CPU, memory usage, and active processes)
8.  df -h - Shows CPU, memory usage, and active processes (Ex:/dev/sda1  100G  50G  50G  50% /)
9.  history - Displays list of previously executed commands (ex:1 pwd, 2 ls, 3 cd SQL, ...)
10. uptime - Shows system uptime, number of users, and load average (ex:20:30:01 up 5 days, 3:20, 2 users, load average: 0.00, 0.01, 0.05)

SECTION 2 – Write the Linux command for the following tasks.

1.  Create a directory called project-files - mkdir project-files
2.  Navigate into the project-files directory - cd project-files
3.  Create a file called notes.txt using vi - vi notes.txt
4.  Display the contents of notes.txt - cat notes.txt
5.  Copy notes.txt to backup.txt - cp notes.txt backup.txt
6.  Show the first 100 lines of a file called logs.txt - head -n 100 logs.txt
7.  Show the last 100 lines of logs.txt - tail -n 100 logs.txt
8.  Check the disk storage usage of the server - df -h
9.  Check the running processes in the system -ps -ef
10. Delete a file called temp.txt - rm temp.txt

SECTION 3 – Concept Questions

1.  What is the difference between > and >> in Linux?
    (>) → Redirects output to a file, overwriting the existing content.
        echo "Hello" > file.txt  # file.txt will only contain "Hello"
    (>>) → Appends output to a file, keeping existing content.
        echo "World" >> file.txt  # "World" will be added at the end of file.txt
2.  What is the purpose of the kill -9 command?
    kill -9 <PID> forcefully terminates a process with the given Process ID.
    -9 sends the SIGKILL signal, which cannot be ignored by the process.
3.  What is the difference between rm and rmdir?
    rm → Deletes files or directories (use -r for directories recursively).
    rmdir → Deletes empty directories only.
4.  What information does the netstat -tulpn command provide?
    Shows active network connections and listening ports.
    -t → TCP, -u → UDP, -l → Listening, -p → Process using port, -n → Show numeric addresses
5.  What is the purpose of the ping command?
    Tests connectivity to a host (IP address or domain) and measures round-trip time.
    ex:ping google.com
    Shows if the server is reachable and the response time

    SECTION 4 – Scenario based Questions

1.  You want to check the current working directory. Which command will you use?
    pwd
2.  You want to create a directory called devops inside the home directory. Write the command.
    mkdir ~/devops
3.  You want to check which process is using high CPU in the system. Which command will help?
    ps -eo pid,ppid,cmd,%mem,%cpu --sort=-%cpu | head
4.  You want to check whether your server can connect to google.com. Which command will you use?
    ping google.com
5.  You want to view the last 50 lines of a log file called application.log. Write the command.
    tail -n 50 application.log
