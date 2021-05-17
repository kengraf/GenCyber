# UNH GenCyber : Wednesday: “Spies and Codes” Lesson Plan
Introduction to Linux security and Python based security programming.

## Lesson Description
Four (4) lessons based on interactive IPython notebooks.  The first lesson covers basic Linux security concepts.  The remaining lessons use Python to investigate steganography, ciphers, and authnetication tokens.

### Prerequisite Knowledge
Students should have a basic understanding of how to use a web browser and be able to engage using remote meeting tools.

### Length of Completion
The lesson has four (4) modules. Each module starts with a brief (15 minute) overview to provide context, instructions, and goals for the students.  Students typically complete each module in 60-90 minutes.  These lessons are based on IPython and use BinderHub and JupyterHub to create interactive environments. The modules have the following sequence.  

*Module 1: [Intro to Linux command line](https://github.com/kengraf/LinuxCommand)*  
This lesson is based on excerpts from "The Linux Command Line" 2nd edition by William Shotts.  
*Module 2: [Using a railfence cipher](https://github.com/kengraf/Railfence)*   
Use the Railfence cipher to encrypt messages that we can shared with other students for them to decrypt.  
If you don't know what a Railfence cipher is, check out the [Wikipedia page for Railfence Cipher](https://en.wikipedia.org/wiki/Rail_fence_cipher)
*Module 3: [Image based steganography](https://github.com/kengraf/Steganography)*   
Camp lesson on pyton programming using image based stenanogrpahy.  
*Module 4: [TOTP (GoogleAuthenicator like) tokens](https://github.com/kengraf/TOTP)*    
Python OTP example that works with Google Authenticator.  
Basic functions to generate and validate TOTP and HOTP codes.
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

All lessons use Jupyter notebooks based on IPython and can launced from [Github](https://github.com/kengraf/GenCyber)
The startup of Binder.org takes a minute or so to establish an IPython environment.
To start he lesson click on the lesson link "LESSON.ipynb".
Feel free to play/alter the steps in the lesson.
You will be working in your own temporary sandbox, so you can not damage the original lesson.

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

Try the following commands from the book
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
```


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
- Railfence is sometimes called a zig-zag cipher
- Jupyter notebooks present a set of cells.  The cells should be executed in sequencial order.

Discussion: Consider the "math"?
- What are the minimum and maximum number of rails?
- What is the largest effective offset?
- How many attempts would a brute force require?

Instructions for hands on exercise
- Using a railfence cipher [Binder](https://mybinder.org/v2/gh/kengraf/Railfence/HEAD)
- The startup of Binder.org takes a minute or so to establish an IPython environment.
- To start he lesson click on the lesson link "LESSON.ipynb".
- Feel free to play/alter the steps in the lesson.
- You will be working in your own temporary sandbox, so you can not damage the original lesson.

Lesson text
# Railfence Lesson
In this lesson we use the Railfence cipher to encrypt messages that we can shared with other students form them to decrypt.  
If you don't know what a Railfence cipher is, check out the Wikipedia page. 
[Wikipedia page for Railfence Cipher](https://en.wikipedia.org/wiki/Rail_fence_cipher)


```python
# Run this cell first.  As it initializes the python module
# containing the functions this lesson requires

import railfence
```

Didn't see anything happen? Good!  
  
That means the python runtime located and loaded the module.  
The railfence.py module is located in this repository so locating it is pretty easy for the runtime.


```python
# Run this module to see what happens when a module can't be located
# Any errors later in the lesson will have similar output
import icalledthismodulemoonbeam
```
ModuleNotFoundError: No module named 'icalledthismodulemoonbeam'

```python
# When you run this cell it will encrypt an origial message and display your secret message.

originalMessage = "People say nothing is impossible, but I do nothing every day - A. A. Milne"
secretMessage = railfence.encrypt(originalMessage)
print(secretMessage)
```

Plaonspi,tdonv  . nepesyntigi mosbe u  ontigeeydy-A .Mleo  h islbI h ra Ai


```python
# Then it decrypt the secret message returning a solved message.

solvedMessage = railfence.decrypt(secretMessage)
print(solvedMessage)
```

   People say nothing is impossible, but I do nothing every day - A. A. Milne



```python
# We can now test to compare the original message with the solved message.

if(originalMessage == solvedMessage):
    print( "Solved.  Good job!")
else:
    print("Oh, no?!")
```

Solved.  Good job!


####  It is your turn, secret #1
1) Change the original  message and rerun the cell to generate a new secret message.  
2) Post the secret message to your Discord channel as secret message #1.  
3) Copy the secret message from another camper's channel.  
4) Decrypt the secret message.  
5) Does the solved message look correct?  


```python
# add your fun quote or message to the string

originalMessage = "" 
print( railfence.encrypt(originalMessage) )
```

    



```python
# Paste a secret from someone
# does the output make sense?

secretMessage = "" 
print(railfence.decrypt(secretMessage))
```

    


#### Changing the number of rails, secret #2
Railfences can have different numbers of rails.  
So far you have used the module's default value of 3 rails.  

Let's do a other sharing experiment this time picking the number of rails.


```python
# Change the number of rails (use a value less than 8 and not 3)
railCount = 3
print( railfence.encrypt(originalMessage, railCount) )
```

    



```python
secretMessage = "" # add the secret in the quotes
railCount = 3 # You may need to make a few guesses (2-7), because you don't know the actual number
print(railfence.decrypt(secretMessage, railCount))
```

    


#### Starting on a different rail, secret #3
You start anywhere in a rail cycle.
So far, we have using the default value of starting on the first rail (offset = 0)

Same sharing process as before, this time changing the offset.


```python
offset = 0 # Change the offset to something not zero
print( railfence.encrypt(originalMessage, 3, offset) )
```

    



```python
secretMessage = "" # add the secret in the quotes
offset = 0 # You will need to make a few guesses, because you don't know the actual number
print(railfence.decrypt(secretMessage, 3, offset))
```

    


#### Making it harder, secret #4
This last share we are going to try harder on humans to decrypt the message.

Pick both the number of rails and an offset.  Even for single digit values you are creating dozens of possibilities.


```python
railCount = 0 # Change the value
offset = 0 # Change the value
print( railfence.encrypt(originalMessage, railCount, offset) )
```

    



```python
secretMessage = "" # add the secret in the quotes
railCount = 0 # You will need to make a few guesses
offset = 0 # even more guesses
print(railfence.decrypt(secretMessage, railCount, offset))
```

    


#### Let the computer do the iterations for you


```python
secretMessage = "" # add the secret in the quotes

for railCount in range(2, len(secretMessage)//2):
    cycleSize = railCount + railCount - 2
    for offset in range(0, cycleSize):
        maybeSolution = railfence.decrypt(secretMessage, railCount, offset)
        print("Rails=%d, Offset=%d, maybe=%s" % (railCount, offset, maybeSolution ))
```

#### Extra credit, have the computer pick the best solution
What if you scored every maybeSolution for the number of actual words it contains?  
Then only print the best solution, rather than showing all iterations?

You would need to load a dictionary of words [Google's 10,000 most common](https://github.com/first20hours/google-10000-english)
Then try to match the words in the dictionary  to the words in your maybeSolution.

Extra-extra credit: For really large messages or dictionaries you may want to consider sorting the wordlists to be computationally efficient.

Wrap up
- Clone the repo: git clone https://github.com/kengraf/Railfence.git  
- Web enable railfence.py  

### Module 3: Image based steganography
Points to be stressed during the lesson
- Hiding messages in images is easy. Lots of bits that the human eye isn't going to notice.
- It is best to start with an image that has a range of colors and avoids solid backgrounds.
- Let's start with a depiction of the Charge of the Light Brigage, in real-life spies would use candid shots.

Discussion: Could a computer notice the message?
- Use Google image/search to compare images?
- Analyse low order bits for a pattern?
- If you use encryption does sharing the keys become the weak link?

Instructions for hands on exercise
- Camp lesson on pyton programming using image based stenanogrpahy.  
- The audience isn't expected to be programming or security knowledgeable.
- How to use image based steganogrpahy [Binder](https://mybinder.org/v2/gh/kengraf/Steganography/HEAD)  
- The startup of Binder.org takes a minute or so to establish an IPython environment.  
- To start he lesson click on the lesson link ".ipynb".   
- Feel free to play/alter the steps in the lesson. You will be working a temporary sandbox, so can not damage the original lesson.  

# Steganography lesson
Hiding messages in images is easy.  Lots of bits and the human eye isn't going to notice.  
Could a computer notice?  Let's see.

It is best to start with an image that has a range of colors and avoids solid backgrounds.

Let's use a depiction of the Charge of the Light Brigage, in real-life spies would use candid shots.

![](Charge600.jpg)

# Before we start let's make sure the software we need is installed correctly
# All the tests should show as 'Passed' 
import steganography as steg
steg.selfTest()

# Time now to conceal our message.
# Remember 'steganography' is greek for covered writing.
# While spies would encrypt and cover their message, we are only going to cover.

imageName = "Charge600.jpg"
coveredMessage = "Into the valley of death rode the 600"
colorUsed = 'R'
bitUsed = '1'
image = steg.encode( imageName, coveredMessage, colorUsed + bitUsed )
coverImage = 'hidden.png'
steg.write(coverImage,image)

### Run this cell to show the hidden message image
![](hidden.png)

# Could you see the differrence?   If yes, then you are super human!
# Use the decode function to retrieve the original message

message = steg.decode(coverImage, colorUsed + bitUsed )
print(message)

## Lesson #1
Upload an image you would like to use as your cover image  'your-image-name' 
Set a short message as your "your-message".  Song lyrics, poems, and famous quotes work well.  

imageName = "your-image-name"
coverMessage = "your-message"
colorUsed = 'R'
bitUsed = '1'
image = steg.encode( imageName, coverMessage, colorUsed + bitUsed )
coverImage = 'cover.png'
steg.write(coverImage,image)

### Run this cell to show your hidden message image
![](cover.png)

# 1) Share the cover.pmg in your Discord channel
# 2) upload someone elses image
import urllib.request
targetUrl = "http://unhash.cyber-unh.org/files/22525dbaeff388b36ae3176722cf223b/unhash21.png"
contents = urllib.request.urlopen(targetUrl).read()
print("Loaded %d byes" % (len(contents)))
copiedImage = "lesson1." + targetUrl.split(".")[-1]
with open(copiedImage, 'w') as f:
    f.write(raw)
    f.close()
    print(copiedImage + " saved")

# Find the hidden message
message = steg.decode(coverImage, colorUsed + bitUsed )
print(message)

## Lesson #2
Same process as lesson #1, but this time try a different color and bit
Note if you use bit 8 you might notice a visual change in the image

colorUsed = 'R' # Change this to 'B' or 'G'
bitUsed = '1' # Change the bit layer used (2 thru 8)
image = steg.encode( imageName, coverMessage, colorUsed + bitUsed )
coverImage = 'cover2.png'
steg.write(coverImage,image)

# 1) Share the cover2.pmg in your Discord channel
# 2) upload someone elses image
import urllib.request
targetUrl = "http://unhash.cyber-unh.org/files/22525dbaeff388b36ae3176722cf223b/unhash21.png"
contents = urllib.request.urlopen(targetUrl).read()
print("Loaded %d byes" % (len(contents)))
copiedImage = "lesson1." + targetUrl.split(".")[-1]
with open(copiedImage, 'w') as f:
    f.write(raw)
    f.close()
    print(copiedImage + " saved")

# Find the hidden message
colorUsed = 'R' # You may need a few guesses 'B' or 'G'
bitUsed = '1' # You may need a few guesses (2 thru 8)

message = steg.decode(coverImage, colorUsed + bitUsed )
print(message)

## Extra credit 
The steganography module is not very sophiscated.  Law enforcement might assume you are trying to hide a message read all the low bits and try to see if there is a message.

What would you do to change how the bits are placed in the image?

1) Write multiple colors  
2) Reverse the bit order of the message  
3) Start is the middle of (or some random place) image  
4) Use an XOR mask  
5) Write as a linked list  
6) Use base64  
...?

Bonus work:
- Post images in your channel for other students to use.
- Clone the repo: git clone https://github.com/kengraf/Steganography.git  
- Web enable or add encryption to steganography.py  


### Module 4: TOTP (GoogleAuthenicator like) tokens

Points to be stressed during the lesson
- 

Discussion: Would any of the following *tricks* make deciphering harder?
- 

Instructions for hands on exercise
- Camp lesson on pyton programming using image based stenanogrpahy.  
- The audience isn't expected to be programming or security knowledgeable.
- How to use image based steganogrpahy [Binder](https://mybinder.org/v2/gh/kengraf/TOTP/HEAD)  
- The startup of Binder.org takes a minute or so to establish an IPython environment.  
- To start he lesson click on the lesson link ".ipynb".   
- Feel free to play/alter the steps in the lesson. You will be working a temporary sandbox, so can not damage the original lesson.  

Bonus work:
- Post messages in your channel for other students to use.
- Clone the repo: git clone https://github.com/kengraf/Steganogrpahy.git  
- Web enable steganography.py  

### Questions/Concerns/Suggestions/Bugs
Please post issues to the [GitHub page](https://github/kengraf/GenCyber)
