# Linux Commands
This is my notes that is prepared by learning the basic commands of linux and th practice snaps have been added to the notes too.

Not all commands work on windows command line, so switching to MAC OS or Ubuntu is a feasible option.
****
## What is Linux command?
Linux command is a program or a utility that runs on the command line. This accepts lines of instruction from the user and processes them into instructions for the computer to process it.
****
## Commands for System Information

1. **Hostname**

This command is used to obtain the DNS (Domain Name System) name and hostname is something that is given to a computer attached to it's network.

![](/2022-09-20-16-56-12.png)

2. **Last Reboot**

This command gives us the history of the users that have logged into this specific system for doing their tasks

![](/2022-09-20-16-57-12.png)

3. **Date**

This command displays today's date in the command terminal. 

![](/2022-09-20-16-59-11.png)

4. **cal**

This command displays the specific month's calendar and as of now it is September 2022.

![](/2022-09-20-17-00-43.png)

5. **w**

This command displays the users that are online and are using the systems.

![](/2022-09-20-17-01-57.png)

6. **whoami**

This command displays who I am logged in as. 

![](/2022-09-20-17-03-20.png)

7. **last**

This command displays the users who logged into this system previously.

![](/2022-09-20-17-05-53.png)

8. **Other System Commands**

The other vital commands to operate the system are **poweroff** (for shutting down the system), **reboot** (for rebooting the system), **logout** (for logging out) and who (to show who logged into the system).

****
## Commands for accessing files and directories

- **Pwd - Print Work Directory**:
It prints the path of the working directory, starting from the root. pwd is shell built-in command(pwd) or an actual binary(/bin/pwd). There are two types of pwd and those are pwd -d  and  pwd -l.

![](/Capture.PNG)

- **Ls - list and generate statistics for files**: 

*ls* is a Linux shell command that lists directory contents of files and directories.

![](/Capture%201.PNG)

- **Ls -a**:
To show all the hidden files in the directory, use ‘-a option’. Hidden files in Unix starts with ‘.’ in its file name.It will show all the files including the ‘.’ (current directory) and ‘..’ (parent directory).

![](2022-09-20-23-47-35.png)

- **Ls -l**:
To show long listing information about the file/directory.

![](2022-09-20-23-50-22.png)

- **Mkdir**
*mkdir* command in Linux allows the user to create directories (also referred to as folders in some operating systems). This command can create multiple directories at once as well as set the permissions for the directories.

*We can notice that a directory named 'f3' is created.*

![](2022-09-20-23-53-01.png)

- **Cd**

*cd* command in linux known as change directory command. It is used to change current working directory.

*We can notice that we have opened 'f3' directory.*

![](2022-09-21-00-01-48.png)

- **Cd ..**

This command is used to move to the parent directory of current directory, or the directory one level up from the current directory. “..” represents parent directory.

*We can notice that we have exited 'f3' directory.*

![](2022-09-21-00-03-58.png) 

- **Cd /**

This command is used to change directory to the root directory, The root directory is the first directory in your filesystem hierarchy.

![](2022-09-21-00-09-48.png)

- **Touch**

It is used to create a file without any content. The file created using touch command is empty. This command can be used when the user doesn’t have data to store at the time of file creation.

*We can notice that 'file1.txt' is created.*

![](2022-09-21-00-14-22.png)

- **Nano**

The above command will open a new file with new_filename as shown in the output. In case the file already exists it will open the same and in case the file is not there in the current directory it will create a new one. At the bottom of the window, there is a list of shortcut keys for nano.

![](2022-09-21-00-17-43.png)

*After typing the command then the console in the picture below opens, we do the necessary tasks and save the text file.*

![](2022-09-21-00-18-13.png)

- **Cat**

Cat(concatenate) command is very frequently used in Linux. It reads data from the file and gives its content as output. It helps us to create, view, and concatenate files. So let us see some frequently used cat commands.

*We can see that the content in the file1.txt file is displayed.*

![](2022-09-21-12-59-43.png)

- **mv**

*mv* stands for move. mv is used to move one or more files or directories from one place to another in a file system like UNIX. It has two distinct functions: 

 *It renames a file or folder.*

![](2022-09-21-13-10-19.png)

- **cp**

*cp* stands for copy. This command is used to copy files or group of files or directory. It creates an exact image of a file on a disk with different file name. cp command require at least two filenames in its arguments.

![](2022-09-21-13-16-43.png)

**Rm**

*rm* stands for remove here. rm command is used to remove objects such as files, directories, symbolic links and so on from the file system like UNIX.

*There is no output because the directory is empty.*

![](2022-09-21-13-48-42.png)

**Rmdir**

*rmdir* command is used remove empty directories from the filesystem in Linux. The rmdir command removes each and every directory specified in the command line only if these directories are empty. So if the specified directory has some directories or files in it then this cannot be removed by rmdir command.

![](2022-09-21-13-50-39.png)

**History**

History command is used to view the previously executed command.

![](2022-09-21-13-51-54.png)

*Last 500 commands are visible on using history command.*

![](2022-09-21-13-52-21.png)

**ifconfig**

ifconfig(interface configuration) command is used to configure the kernel-resident network interfaces. It is used at the boot time to set up the interfaces as necessary.

![](2022-09-21-13-40-48.png)

**iwconfig**

It is used to set the parameters of the network interface that are particular to the wireless operation like SSID, frequency etc. iwconfig may also be used to display the parameters, and the wireless statistics which are extracted from /proc/net/wireless.

*There are no wireless devices connected so the output is this.*

![](2022-09-21-13-41-21.png)

**Ping**

*Ping* command is used to check the network connectivity between host to host or server to host and it doesn’t stop until the user hits ctrl+c until then the data is always posted on the console.

*To stop it we must use ctrl + c.*

![](2022-09-21-13-40-14.png)

**Less**

Less command is a Linux utility that can be used to read the contents of a text file one page(one screen) at a time. It has faster access because if file is large it doesn’t access the complete file, but accesses it page by page. 

![](2022-09-21-13-44-41.png)

*Once you click enter this is what is displayed.*

![](2022-09-21-13-45-43.png)

*To move from this click enter and then click esc.*

**Uname -a**

The command ‘uname‘ displays the information about the system. -a option: It prints all the system information in the following order: Kernel name, network node hostname, kernel release date, kernel version, machine hardware name, hardware platform, operating system.

![](2022-09-21-14-41-53.png)

**Head**

It is the complementary of Tail command. The head command, as the name implies, print the top N number of data of the given input. By default, it prints the first 10 lines of the specified files. If more than one file name is provided then data from each file is preceded by its file name. 

![](2022-09-21-14-45-21.png)

**Tail**

It is the complementary of head command.The tail command, as the name implies, print the last N number of data of the given input. By default it prints the last 10 lines of the specified files. If more than one file name is provided then data from each file is precedes by its file name.

![](2022-09-21-14-47-01.png)

**Just**

Should work on it as it was not working in the system.


**Locate**

*Locate* command in Linux is used to find the files by name. There is two most widely used file searching utilities accessible to users are called find and locate. The locate utility works better and faster than find command counterpart because instead of searching the file system when a file search is initiated, it would look through a database.

![](2022-09-21-14-53-51.png)

**Find**

The find command in UNIX is a command line utility for walking a file hierarchy. It can be used to find files and directories and perform subsequent operations on them. It supports searching by file, folder, name, creation date, modification date, owner and permissions.

![](2022-09-21-14-56-52.png)

**File**

*File* command is used to determine the type of a file. .file type may be of human-readable(e.g. ‘ASCII text’) or MIME type(e.g. ‘text/plain; charset=us-ascii’).

```
File with * icon displays all the file's file type.
```
![](2022-09-21-15-03-50.png)

```
File with -b, –brief : This is used to display just file type in brief mode.
```
![](2022-09-21-15-05-47.png)

```
File Directoryname/* is used to display all files filetypes in particular directory.
```
![](2022-09-21-15-08-31.png)

**More and Page**

*More* command is used to view the text files in the command prompt, displaying one screen at a time in case the file is large (For example log files).

```
-d is used o help the user to navigate.
```

![](2022-09-21-15-19-00.png)

![](2022-09-21-15-19-34.png)

**Chgrp**

*chgrp* command in Linux is used to change the group ownership of a file or directory. All files in Linux belong to an owner and a group.

![](2022-09-21-16-45-41.png)

**Chown**

Different users in the operating system have ownership and permission to ensure that the files are secure and put restrictions on who can modify the contents of the files. In Linux there are different users who use the system:  

```
This command is used to give ownership but the university's system don't permit us to do this.
```

![](2022-09-21-17-11-28.png)

**Chmod**

In Unix-like operating systems, the chmod command is used to change the access mode of a file.
The name is an abbreviation of change mode. 

```
r - Permission to read the file. 
w - Permission to write and delete the file.
x - Permission to execute the file

In the example below the c1.txt file authorization has been changed to read only.
```

![](2022-09-21-17-17-26.png)

--- 