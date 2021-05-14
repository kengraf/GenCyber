# UNH GenCyber : Wednesday: “Spies and Codes” Lesson Plan
Introduction to Linux security and Python based security programming.

## Lesson Description
TBD

### Prerequisite Knowledge
Students should have a basic understanding of how to use a web browser and be able to engage using remote meeting tools.

### Length of Completion
The lesson has four (4) modules. Each module starts with a brief (15 minute) overview to provide context, instructions, and goals for the students.  Students typically complete each module in 60-90 minutes.  These lessons are based on IPython and use BinderHub and JupyterHub to create interactive environments. The modules have the following sequence.  

*Module 1: Intro to Linux command line*  
This lesson is based on excerpts from "The Linux Command Line" 2nd edition by William Shotts. 
*Module 2: Using a railfence cipher*  
TBD
*Module 3: Image based steganography*  
TBD
*Module 4: TOTP (GoogleAuthenicator like) tokens*  
TBD
### Level of Instruction
The lesson is intended for high school learners (beginner and intermediate levels)

## Applicable First Principles and Concepts

### GenCyber First Principles
<table border="0">
 <tr>
  <td><i>Abstraction</i></td>
   <td><i>Data Hiding</i></td>
   <td><i>Domain Separation</i></td>
   <td><i>Layering</i></td>
   <td><i>Least Privilege</i></td>
 </tr>
 <tr>
   <td><i>Minimization</i></td>
   <td>Modularity</td>
   <td>Process Isolation</td>
   <td><i>Encapsulation</i></td>
  <td><i>Simplicity</i></td>
 </tr>
</table>
### GenCyber Cybersecurity Concepts
<table border="0">
 <tr>
  <td>Availability</td>
  <td><i>Confidentiality</i></td>
  <td><i>Defense in Depth</i></td>
 </tr>
 <tr>
  <td><i>Integrity</i></td>
  <td><i>Keep it Simple</i></td>
  <td><i>Think like an Adversary</i></td>
 </tr>
</table>
 
## Resources & Requirements
- Each student needs access to a browser and have the ability to connect to the remote meeting with both video and audio.
- Websites/Software used  
[Secure Shell extension in Google Store](https://chrome.google.com/webstore/detail/secure-shell/iodihamcpbpeioajjeobimgagajmlibd)  
[The Linux Command Line](https://github.com/kengraf/LinuxCommand/blob/main/thelinuxcommandline.pdf)   
[Github](https://github.com/kengraf/LinuxCommand/blob/main/LESSON.ipynb)

## Accommodations Needed
Special technical setup may be needed for students who are visually or physically impaired to use the
computer or engage in a remote meeting.

## LEARNING OUTCOMES
- Demonstrate the ability to configure secure logins to a Linux machine
- Demonstrate the ability to use Linux commands.
- Programmaticaly Create secure authentication tokens
- Embed secret messages inside a image

## LESSON DETAILS
### Assessment
The assessment for this lesson is a combination of informal observation and game statistics:
- The number of students answering using SSH keys for logins
- The number of students creating secret messages based on steganography
- THe number of the students demonstrating the ability to generate TOTP tokens

### Differentiated Learning Opportunities
Hands-on exercise provides a base challenge and one or more bonus challenges.  
Online resources are provided for self-paced study.

## LESSON PREPARATION
### General
Students need accounts setup on kali.cyber-unh.org  
Initial password is "CHANGE.me", which must be changed on first login

### SOFTWARE
This lessons uses online resources.  The only software install is a browser extension (Chromebooks only).
[Secure Shell extension in Google Store](https://chrome.google.com/webstore/detail/secure-shell/iodihamcpbpeioajjeobimgagajmlibd)  

## LESSON 
### Module 1: Intro to Linux command line
This lesson uses excerpts from [The Linux Command Line]([The Linux Command Line](https://github.com/kengraf/LinuxCommand/blob/main/thelinuxcommandline.pdf)   
 2nd edition by William Shotts.  

Students are encouraged to learn from the entire book.  
This lesson is focused learning about basic Linux security (Chapter 9: Permissions) and (Chapter 16:Networking).  
We will briefly cover Chapters 1-6 for students completely new to Linux.

Validate connectivity
- In a terminal window: ssh <username>@kali.cyber-unh.org
- If command not found install the browser extension to login  

# Introduction to Linux
This lessons uses excerpts from "The Linux Command Line" 2nd edition by William Shotts. Camp instructions will tell how to obtain the book.

Students are encouraged to learn from the entire book.  This lessons is focused learning about basic Linux security (Chapter 9: Permissions) and (Chapter 16:Networking).  We will briefly cover Chapters 1-6 for students completely new to Linux.

## Connecting to Linux system
The camp will provide access to a Linux system.  Specifically it is an instance of Kali running in AWS.  Login instructions will be provided in your camp materials. 

Connecting to the Linux system requires the use of SSH.  The Chrome browser extension "Secure Shell" will allow you to access the Linux from within your browser. 
[Secure Shell extension in Google Store](https://chrome.google.com/webstore/detail/secure-shell/iodihamcpbpeioajjeobimgagajmlibd)




## Chapter 1: What is the shell?
The shell prompt look something like this:  
`┌──(ken㉿kali)-[~]`  
`└─$`  
It shows the user's name `ken` the machine name `kali` and your current working directory `~` which is a shortcut for your home directory or `/home/ken` for user `ken`

Try some basic commands  
- data  
- cal  
- df  
- free  

Keyboard shortcuts  
- After typing enough of a command or filename to make it unique you can use the `tab` key to complete.  
- The `up arrow` can be used to recall past commands  
- The `history` command will your past commands
- `!!` will execute the last command in your history    
- `!#` will execute the command numbered in your history  
- `!name` will execute the last command strating with `name`

While using history can be convenient, you need to remember that if you type passwords or other secrets on the command line they be remembered in your history and potentially visible to other users.


## Chapter 2: Navigation

- `pwd` Print name of current working directory  
- `cd` Change directory  
- `ls` List directory contents  

Try the follwoing commands from the book
```
pwd
ls
cd /usr/bin
ls
cd /usr
pwd
cd ..
pwd
cd ./usr
pwd
cd ./bin


## Chapter 3: Exploring the system
- `ls` List directory contents  
- `file` Determine file type  
- `less` View file contents  

Try the follwoing commands from the book
```
ls
ls /usr
ls ~ /usr
ls -l
ls -lt
ls -lt --reverse
file .
file /etc/passwd
less /etc/passwd
```

## Chapter 4: Manipulating Files and Directories
- `cp` Copy files and directories  
- `mv` Move/rename files and directories  
- `mkdir` Create directories  
- `rm` Remove files and directories  

Try the following commands
```
mkdir dir1
echo "some text" > item1
cp item1 item2
cp item2 dir1
mv item1 item2
mv item2 dir1
cd dir1
rm item1
cd ..
rm -r dir1


## Chapter 5: Working with commands
- `type` Indicate how a command name is interpreted  
- `which` Display which executable program will be executed  
- `help` Get help for shell builtins  
- `man` Display a command’s manual page  
- `apropos` Display a list of appropriate commands  
- `info` Display a command’s info entry  
- `whatis` Display one-line manual page descriptions  
- `alias` Create an alias for a command  

Try the following commands
```
type type
type ls
type cp
which ls
which cd
help cd
mkdir --help
man ls
man 5 passwd
apropos partition
whatis ls
info ls
```

## Chapter 6: Redirection
- `cat` Concatenate files  
- `sort` Sort lines of text  
- `uniq` Report or omit repeated lines  
- `grep` Print lines matching a pattern  
- `wc` Print newline, word, and byte counts for each file  
- `head` Output the first part of a file  
- `tail` Output the last part of a file  
- `tee` Read from standard input and write to standard output and files  

Try the following commands
```
ls -l /usr/bin > ls-output.txt
ls -l ls-output.txt
less ls-output.txt
ls -l /usr/bin | less
ls -l /usr/bin | sort | less
ls /usr/bin | sort | less
ls /usr/bin | sort | uniq | grep zip
ls -l /usr/bin > ls-output.txt
head -n 5 ls-output.txt
tail -n 5 ls-output.txt
history
```

## Chapter 9: Permissions
- `id` Display user identity  
- `chmod` Change a file’s mode  
- `umask` Set the default file permissions  
- `su` Run a shell as another user  
- `sudo` Execute a command as another user  
- `chown` Change a file’s owner  
- `chgrp` Change a file’s group ownership  
- `passwd` Change a user’s password  

Try the following commands
```
file /etc/shadow
less /etc/shadow
id
> foo.txt
ls -l foo.txt
chmod 600 foo.txt
ls -l foo.txt
rm -f foo.txt
umask
> foo.txt
ls -l foo.txt
rm foo.txt
umask 0000
> foo.txt
ls -l foo.txt
```

## Chapter 16: Networking
- `ping` Send an ICMP ECHO_REQUEST to network hosts  
- `traceroute` Print the route packets trace to a network host  
- `ip` Show/manipulate routing, devices, policy routing, and tunnels  
- `netstat` Print network connections, routing tables, interface statistics  
- `wget` Non-interactive network downloader  
- `ssh` OpenSSH SSH client (remote login program)  

Try the following commands from the book
```
ping linuxcommand.org
traceroute slashdot.org
ip a
netstat -ie
netstat -r
wget http://linuxcommand.org/index.php
```
ssh ken@localhost
```

## Sharing Files (local & remote)
This exercise explores file permissions and is not in the book.  

There is a user `peppapig`on the system. She is friendly (and not so serious about security) and shares readable and writable files and directories.  The following commands look at a few ways you interact with Peppa's files.  

The first step all attackers is recon.  These commands allow us to move to Peppa's home directory (often home directories are readable).  We can read some files.  Can you explain the difference in file permissions?  If not, the book will help.

```
cd /home/peppapig
ls -l
more public_quote
more private_quote
```
Reading files in another user's home directory happens when all the users on that system are collaborating as team.  Not good for privacy but great for sharing.  
Should we be able to write things into Peppa's home directory?

The next commands show we can.  Can you explain why?

```
echo "O George!" > myname.quote
echo "O George!" > studentPlayground/myname.quote
ls studentPlayground/
```

OK, back to your home directory.  In the "old days" we used FTP.  Passwords in the clear, bad, Bad, BAD! Today, we use scp.  It works like the `cp` command but allows use to copy from/to other systems like FTP.  
`cp sourceFile destinationFile`
scp adds user@host:
`scp user@host:sourceFile user@host:destinationFile`

The following commands all have the same result, if you are user `george` working in george's home directory.  
Give a few a try, replacing "ken" with your username.

```
cd ~
cp /home/peppapig/public_quote /home/george/mycopy
cp /home/peppapig/public_quote mycopy
scp george@kali.cyberunh.org:/home/peppapig/public_quote george@kali.cyberunh.org:/home/george/mycopy
scp kali.cyberunh.org:/home/peppapig/public_quote george@kali.cyberunh.org:mycopy
scp george@kali.cyberunh.org:~/../peppapig/public_quote mycopy
scp kali.cyberunh.org:/home/peppapig/public_quote .

```
You can also use scp to write, assuming you have the permissions.   
Create a file with a fun quote in your home directory than move it to Peppa's playground folder.
```
cd ~
echo "Add a fun quote here" > george.quote
scp george.quote kali.cyberunh.org:studentPlayground/
```
Did your quote show up in the playground?
```
ls -l /home/peppapig/studentPlayground/
```

### Extra-credit:
Can other users read the contents of your home directory?  Can you prevent that?


Can you make any of the following commands work?  Again, replacing `george` with your username.
```
scp george.quote peppapig@kali.cyberunh.org:studentPlayground/
scp george.quote george@kali.cyberunh.org:/home/peggapig/studentPlayground/
su peppapig
ssh peppapig@kali.cyber-unh.org
```

## Cracking Passwords
When passwords are stored they are hashed.  The math behind hashing is a Ph.D. level discussion.  What we need to know is:
1) MD5 and SHA are good time-tested algorithms
2) Hash algorithms reduce a (file|string) to a unique and small set of bits
3) The hash algorithm is not reversable

This makes hashing great for storing passwords.  If attackers get the password list they can't reverse the hash to get the password.  With one BIG caveat. Your password is unique enough that someone hasn't put the hash of your password in a in list.

The MD5 hash of `password` is `5f4dcc3b5aa765d61d8327deb882cf99`.  Google the hash and now you know the origin is `password`

The commands below hash a number of strings using MD5.  Storing all the hashes in a file.  We add `.salted` to a few password as some randomish text to hopefully fool Google and cracking tools.  
```
echo -n "george" | md5sum > hashes
echo -n "george.salted" | md5sum >> hashes
echo -n "badpassword" | md5sum >> hashes
echo -n "password" | md5sum >> hashes
echo -n "password.salted" | md5sum >> hashes
more hashes
```
The tool we going to use to guess the passwords is John the Ripper.    We have a small clean up edit to put your hash file into a format John likes.  The `rockyou.txt` file is a list of the 14 million most popular passwords. 
```
sed -i 's/ -//g' hashes
more hashes
john --wordlist=/usr/share/wordlists/rockyou.txt --format=Raw-MD5 hashes
more ~/.john/john.pot
```
Which passwords did John find?



## Extra credit 

Bonus work: Hash your goto password.  Does Google or John crack it?

Bonus work: Use SSH keys to login
- cd ~
- ssh-keygen
- cd .ssh
- cp id-rsa.pub authorized_keys
- cat id_rsa 
- # cut/paste the cat output to local system <somefile>
- <somefile> must be protected so that it is only be readable by you
- Validate login:  ssh -i <somefile> <username>@kali.cyber-unh.org

### Module 2: Using a railfence cipher
Points to be stressed during the lesson
- 

Discussion: Would any of the following *tricks* make deciphering harder?
- 

Instructions for hands on exercise
- 

Bonus work: A second message for students that finish quickly
-

Wrap up
- 
### Module 3: Image based steganography
Points to be stressed during the lesson
- 

Discussion: Would any of the following *tricks* make deciphering harder?
- 

Instructions for hands on exercise
- 

Bonus work: A second message for students that finish quickly
-

Wrap up
- 

### Module 4: TOTP (GoogleAuthenicator like) tokens

Points to be stressed during the lesson
- 

Discussion: Would any of the following *tricks* make deciphering harder?
- 

Instructions for hands on exercise
- 

Bonus work: A second message for students that finish quickly
-

Wrap up
- 

### Questions/Concerns/Suggestions/Bugs
Please post issues to the [GitHub page](https://github/kengraf/GenCyber)
