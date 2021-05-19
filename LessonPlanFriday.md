# UNH GenCyber : Friday: “Cryptopuzzles” Lesson Plan
As the final day of camp students will use the lessons learned to complete series of CTF challenges.  Using a Jeopardy like format covering: Crypto, Coding, Web, networking, and Career topics. 

## Lesson Description
Sixty (60) challenge [web site](http://unhash.cyber-unh.org) based on [CTFd](https://github.com/CTFd/CTFd).  The challenges draw from all 4 previous days of camp.

### Prerequisite Knowledge
Students should have a basic understanding of how to use a web browser and be able to engage using remote meeting tools.

### Length of Completion
The lesson is a day long review of what was taught during the week. The format is CTF based, requiring students to use from knowledge gained earlier in the week.

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
   <td><i>Modularity</i></td>
   <td><i>Process Isolation</i></td>
   <td><i>Encapsulation</i></td>
  <td><i>Simplicity</i></td>
 </tr>
</table>
### GenCyber Cybersecurity Concepts
<table border="0">
 <tr>
  <td><i>Availability</i></td>
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
[Challenge web site](http://unhash.cyber-unh.org)  
[Cyber Chef](https://gchq.github.io/CyberChef/)

## Accommodations Needed
Special technical setup may be needed for students who are visually or physically impaired to use the
computer or engage in a remote meeting.

## LEARNING OUTCOMES
- Demonstrate the ability to think like an adversary and identify what can go wrong on a website
- Demonstrate the ability to use Internet resources to gather relevant information.
- Apply knowledge about different types of ciphers.
- Learn the about cybersecurity career resources.

## LESSON DETAILS
### Assessment
The assessment for this lesson is a combination of informal observation and game statistics:
- The number of students correctly answering challenges.

### Differentiated Learning Opportunities
Advanced students will have the opportunity to create their own challenges.  

## LESSON PREPARATION
### General
Validate instructor and student connectivity.  
Instructor should review the hints to understand how each challenge can be solved.  This is especially import for the harder challenges.  

### SOFTWARE
No local software installs are needed.  

## LESSON 
### Category: Sanity  
Just a validity check to make sure everyone knows how to submit a flag (right answer)
```json
{
   "Title": "My first flag",
   "Description": "Flags are case insensitive\nUnless you are told otherwise flags are given in this format flag{my 1st flag}.\nBrute forcing is never the correct approach.\n\nThis message contains the flag for this puzzle.  \n\nGood luck and happy hunting!",
   "Answer": "my 1st flag",
   "Points": 1
 }
```

### Category: Careers  
A set of career resources the students should be aware of.  Nothing tricky in this category; click the link, read the resource, get the answer.
```json
{
   "Title": "Get a job",
   "Description": "What some parents say when asked for money.  Again!\n\nNational Initiative for Cybersecurity Careers and Studies jobs can be found at what web site?",
   "Answer": "niccs.cisa.gov",
   "Points": 10
 }
```
```json
{ 
   "Title": "NIST",
   "Description": "According to the NICE Cybersecurity Workforce Framework document, this category can identify, analyze, and mitigate threats to internal information technology (IT) systems and/or networks.\n\nhttps://niccs.us-cert.gov/workforce-development/cyber-security-workforce-framework\n",
   "Answer": "Protect and Defend",
   "Points": 10
 }
```
```json
{
   "Title": "New collar security",
   "Description": "IBM provides a \"new collar security assessment\" at what site?",
   "Answer": "https://www.ibm.com/training/newcollar",
   "Points": 10
 }
```
```json
{
   "Title": "Interns",
   "Description": "What site says: \"Interns will have the opportunity to apply concepts, protocols and tools acquired through coursework in the real world by working side by side with experts in cybersecurity.\" ?",
   "Answer": "https://www.dhs.gov/homeland-security-careers/cybersecurity-internship-program",
   "Points": 10
 }
```
```json
{
   "Title": "Cyber Safety Series_1",
   "Description": "What is the narrators strong password in the CYBER.ORG Making Strong Passwords video?\nhttps://youtu.be/OiQKZWNeAjc\n",
   "Answer": "T@k0sAPR>>!<3",
   "Points": 20
 }
```
```json
{
   "Title": "Cyber Safety Series_2",
   "Description": "In what city does player 2 live in the CYBER.ORG Online Gaming Safety video? https://youtu.be/V1b4odH-20g ",
   "Answer": "Bossier City",
   "Points": 20
 }
```
```json
{
   "Title": "Cyber Safety Series_3",
   "Description": "What is Person3's password for their bank account in the CYBER.ORG Video Call Safety video? https://youtu.be/m-Sy92NjFmY ",
   "Answer": "Password1234",
   "Points": 20
 }
```
```json
{
   "Title": "Cyber Safety Series_4",
   "Description": "What is the fake banking website that the user ended up at in the CYBER.ORG Phishing video? https://youtu.be/08oJtFFH6a0 ",
   "Answer": "Kingfisherbank.com",
   "Points": 20
 }
```
### Category: Coding  
Majority are logic and numeric base questions.  A few program execution challenges.  
```json
{
   "Title": "Grades",
   "Description": "If I told you your grade was 0x41. What would it mean to your grandmother?",
   "Answer": "A",
   "Points": 1
 }
```
```json
{
   "Title": "bin-2-dec",
   "Description": "Convert the binary number 1010101 to decimal.",
   "Answer": "85",
   "Points": 5
 }
```
```json
{
   "Title": "runme",
   "Description": "Execute runme to reveal the flag. ",
   "Answer": "runtime",
   "Points": 5
 }
```
```json
{
   "Title": "Zen",
   "Description": "Open a command prompt on your machine, run \"python\" to start the Python interpreter, enter \"import this\".\nWhat \"counts\" in Python?",
   "Answer": "Readability",
   "Points": 5
 }
```
```json
{
   "Title": "Counting",
   "Description": "My professor gave me the weirdest math problem today. He told me to add and subtract these numbers, but I can't make heads or tails of it.\n\n01101111 + 01000110 - 01011010 = ??\n\nNote: The flag is the answer to the problem.",
   "Answer": "1011011",
   "Points": 10
 }
```
```json
{
   "Title": "Counting 2",
   "Description": "The honors professor claimed that only 5% of people can solve this math problem. He told us to present the answer next class in decimal format.\n\n0xDD0000 + 0x2A005E0 - 0x04 = \n\nPractical Hint: Base address + Offset address - Padding = ",
   "Answer": "0x37d05dc",
   "Points": 10
 }
```
```json
{
   "Title": "Needs fixing",
   "Description": "This Python script will reveal the flag, but we can't get it to run. See if you can fix it? ",
   "Answer": "nice_job!",
   "Points": 15
 }
```
```json
{
   "Title": "Turducken",
   "Description": "I think I compressed the flag.",
   "Answer": "flag{utqy_HMNT_9915}",
   "Points": 20
 }
```
```json
{
   "Title": "Odd One Out",
   "Description": "I know the flag is in here *once*. But which one is it?",
   "Answer": "wdgw_IQOA_0714",
   "Points": 30
 }
```
```json
{
   "Title": "Bad permissions",
   "Description": "From: Endpoint Security\nSent: Wednesday, July 10th, 2020 2:01 PM\nTo: Alice Cooper\nSubject: File Permission Misconfiguration\n\nHello Alice,\n\nWe recently discovered numerous files with unsafe file permissions on the server. Can you delete all the files and folders where the \"other\" file permission has read, write, and execute permissions set simultaneously (*******rwx). \nOnce you're done please run the provided script to generate your hash for confirmation. Do not change anything else or your generated hash may be incorrect.\n\nThanks,\nEPS\n\nP.S. Extract the archive using the command \"tar -zxvf ./userfiles.tar.gz\"",
   "Answer": "90c560a2049537d2984cb798bcf30d37",
   "Points": 40
 }
```
### Category: Crypto  
[Cyber Chef](https://gchq.github.io/CyberChef) is a good tool for most of these challenges.
```json
{
   "Title": "What is the password",
   "Description": "We've been brought in to assist a police investigation. The detectives took photographic evidence of the suspect's computer systems but were unable to obtain further digital evidence without the password.\nCan you assist the detectives by guessing the password?  Of course, passwords are case-sensitive\n",
   "Answer": "2secret4u",
   "Points": 5
 }
```
```json
{
   "Title": "Password 2",
   "Description": "We've been brought in to assist a police investigation. The detectives took photographic evidence of the suspect's computer systems, but were unable to obtain further digital evidence without the password.\nCan you assist the detectives by guessing the password?",
   "Answer": "dell",
   "Points": 10
 }
```
```json
{
   "Title": "base",
   "Description": "Little Jonney's Secrets for Aspiring Scouts' challenge card gave me this set of characters. I wonder what it means?\n\nZmxhZ3tkcmlua30=",
   "Answer": "drink",
   "Points": 10
 }
```
```json
{
   "Title": "base again",
   "Description": "I was given this abnormal set of characters on my Little Jonney's Secrets for Aspiring Scouts' challenge card. I need to figure it out!\n\nMZWGCZ33N53GC3DUNFXGK7I",
   "Answer": "ovaltine",
   "Points": 10
 }
```
```json
{
   "Title": "Complexity",
   "Description": "How many 8 character passwords are possible using: \n\t\n- These lower-case letters [f, l, a, g]\n- Numerical digits: [0-9] \n- Only these special characters: [ !, @, &]\n\nNotes: \n\n- Other punctuation and special characters are not allowed (e.g. %, $, _, etc.)\n- Submit the answer in this format: flag{NUMBER} Example: flag{123} or flag{24}, etc.",
   "Answer": "6975757441",
   "Points": 10
 }
```
```json
{
   "Title": "hash-ish",
   "Description": "67bcb9695330ca0f2437abb36fc54103",
   "Answer": "greengrass",
   "Points": 10
 }
```
```json
{
   "Title": "Romans",
   "Description": "X_pb_cdi_p_hpaps - this strange text was found on the back of an old roman coin in the back of an evidence room. Can you work out what it means?",
   "Answer": "snickers",
   "Points": 10
 }
```
```json
{
   "Title": "Strange Markings",
   "Description": "Hmm, I'm no expert, but I'm pretty sure those are letters.\nIt kinda looks like it could be a flag but the letters got kabobbled.\n\n... Yeeaaahhh, definitely letters...",
   "Answer": "service over self",
   "Points": 14
 }
```
```json
{
   "Title": "Regular",
   "Description": "There's a flag somewhere in this file. Can you find it?",
   "Answer": "eqim_GMRO_1053",
   "Points": 15
 }
```
```json
{
   "Title": "Kicking the door",
   "Description": "There's something rather strange about this GIF file.  See if you can break it down at work out what it is.",
   "Answer": "splitting_gifs_like_door_frames",
   "Points": 20
 }
```
```json
{
   "Title": "Password String",
   "Description": "Can you figure out the password to get the flag?",
   "Answer": "wktg_QINC_3521",
   "Points": 20
 }
```
```json
{
   "Title": "what does the cat say",
   "Description": "This clever cat picture includes a hidden message. \nHint: passphrase = \"passphrase\"",
   "Answer": "the_hanafuda_captain",
   "Points": 30
 }
```
```json
{
   "Title": "getintothedb",
   "Description": "Hey, the penetration test has been successful so far but we are running out of time! We finally got root \naccess but to impress this client, we really need to demonstrate that we were able to access the accounting \ndatabase. Can you help us find the password for the \"oracle\" user ID?\n\nThe company enforces a password length of 12-characters and a mandatory password change every 30 days. But, \nwe found some notes from the DBA and they have just been incrementing the same password each time! Some of \nthe previous passwords used were \"Database0002\", \"Database1258\", \"Database1400\". If they are still using\nthis scheme, we may be in luck ?\n\nWe pulled a hashed copy of the current passwords from /etc/passwd and /etc/shadow \n\n# cat /etc/passwd\nroot:x:0:0:root:/root:/bin/bash\noracle:x:1000:1000::/home/oracle:/bin/sh\nadmin1:x:1001:1001::/home/admin1:/bin/sh\nuser2:x:1002:1002::/home/user2:/bin/sh\nuser3:x:1003:1003::/home/user3:/bin/sh\nsvcact:x:1004:1004::/home/svcact:/bin/sh\nadmin2:x:1005:1005::/home/admin2:/bin/sh\n\n# cat /etc/shadow\n\nroot:$6$bJ.W.KLYUo13y0Xa$n3h7sxftHqCQA/.EXQtikV.Php9I663yk1qZMX0WJtDaeepqpzEllftQa/AEENPSukozdt7EhJRXvThMQdvF21:18048:0:99999:7:::\noracle:$6$ZP4htNzWSgOj5QXX$fHNKSc2YmjtskceUOWuuzpsHKfro9bhZtCTtYgO2lEhqnNR1RgdYtLDJIn4aE5x6jzXZeybARuRrVNgAVvwKU/:18048:0:99999:7:::\nadmin1:$6$RNFXM4.v$HaVVAyYHRhIjP4GYKRE10Nz3YGd7OiFoatEzjINfXd5tsmRnHdXea5uOb5KFkoYSlhdNqLat6CTwBOfCTpiwH.:18045:0:99999:7:::\nuser2:$6$vd.ACYQd$wIflRf7Qn7Le1hC20XN0i16s2Q/6vls0cvJ8lPEelMwH0Wx8JHXxYurXz6gtqaTkEGU1qDoVJJF0uianU9SAb1:18045:0:99999:7:::\nuser3:$6$EExBiFuA$Q8ej5qSqZI2vK6EieQVzg1yREjUHcDdgoQWenwDgLtoaw2L/O78UoAmSAroOxS.EktBD6v5vUO33TwzcccPcR/:18045:0:99999:7:::\nsvcact:$6$kdDLDay7$1zp2NwSyzEfVBx.iVgwQ4ntx8mzNN1V2C5cN6cKq8umhXcR5DzqVDObz3inPVd1P/SIRaqhHHl/TC2KVYl1fo.:18045:0:99999:7:::\nadmin2:$6$bdEFrPob$LZ/pQ315u8MoKWEUQufOLG9BiecWQfop1rPG6JeCLlNzI0lDJbuDVU0Qv2WJ8TDE0AxT1zpt04Gz0LPmIhkHp.:18045:0:99999:7:::\n\nWhen you find the password for the \"oracle\" user, please send it to us in the flag{password} format.\n\nGood luck!\n",
   "Answer": "Database6419",
   "Points": 40
 }
```
```json
{
   "Title": "mygeneratedwaifu",
   "Description": "Isn't she adorable? She looks so familiar, but I can't figure out where she's from.",
   "Answer": "make.girls.moe",
   "Points": 40
 }
```
```json
{
   "Title": "squarecode",
   "Description": "Get the flag from this mess of pixels.",
   "Answer": "a_few_pixels_go_a_long_way",
   "Points": 40
 }
```
```json
{
   "Title": "keygen",
   "Description": "You have 9 cryptographic public keys.\nThe key generator was optimized by making the prime generation faster, but it is prone to reuse primes.\nCan you find the private key and decrypt the flag?",
   "Answer": "flag{asdfasdfasda}",
   "Points": 50
 }
```
```json
{
   "Title": "stego",
   "Description": "My picture got messed up. Maybe you can fix it for me?\n",
   "Answer": "unbreakable",
   "Points": 50
 }
```
### Category: Networking  
Mostly protocol and TCP/IP addressing.  

```json
{
   "Title": "No place like home",
   "Description": "\"A loopback address is a type of IP address that is used to test the communication or transportation medium on a local network card and/or for testing network applications. Data packets sent on a loopback address are re-routed back to the originating node without any alteration or modification.\"\n\nWhich IP is used for the loopback address? \n\nAnswer format: flag{0.0.0.0}",
   "Answer": "127.0.0.1",
   "Points": 5
 }
```
```json
{
   "Title": "SSH",
   "Description": "What is the standard port for Secure Shell (SSH)?\n\nAnswer format:  flag{00}",
   "Answer": "22",
   "Points": 5
 }
```
```json
{
  "Title": "IPv6",
   "Description": "What is the full, unshortened version of the IP address 1200:2552:AB00:1234::7777:1313?",
   "Answer": "1200:2552:AB00:1234:0000:0000:7777:1313",
   "Points": 5
 }
```
```json
{
   "Title": "txt",
   "Description": "The domain flag.cyber-unh.org has been identified as a domain that's used to pass information around between hackers. There appears to be no website there however, can you find how they're communicating?",
   "Answer": "dns_is_a_great_source_of_data",
   "Points": 10
 }
```
```json
{
   "Title": "AUTH log",
   "Description": "Our primary server has been acting unusual recently. Can you determine the username of the last successful SSH login\n",
   "Answer": "ec2-user",
   "Points": 20
 }
```
```json
{
   "Category": "Networking",
   "Title": "ScanMe",
   "Description": "Which netbios UDP ports are open on the scanme.org server?\nAnswer format:  flag{00,00,00}",
   "Answer": "137,138,139",
   "Points": 20
 }
```
```json
{
   "Title": "Secrets",
   "Description": "What is the password?",
   "Answer": "supersecretpassword",
   "Points": 30
 }
```
```json
{
   "Title": "Too much traffic",
   "Description": "We have been noticing high amounts of traffic going across the network.\nWe believe that a malicious actor is trying to DOS one of our servers. Can you take a look at this packet capture and give us the IP of the attacker so we can block it at the firewall? The victim's IP is 192.168.0.102.",
   "Answer": "11.12.13.14",
   "Points": 30
 }
```

### Category: Trivia  
Most answers can be found using Google.  

```json
{
   "Title": "bookclub",
   "Description": "What is the URL of the \"Rock & Roll Hall of Fame for Cybersecurity Books\" ?  A long list of books now hosted by a university.\n\nAnswer format:  URL",
   "Answer": "https://cybercanon.paloaltonetworks.com/",
   "Points": 5
 }
```
```json
{
   "Title": "classics-101",
   "Description": "Description: In 1989 a Berkeley National Laboratory astronomer became curious about a $0.75 accounting\ndiscrepancy in the computer usage logs and launched an investigation eventually leading to the arrest of a hacker in Europe. \n\nWhat is the name of the classic cybersecurity book he wrote? (answer format: flag{The Xxxxxx'x Xxx} )",
   "Answer": "the cuckoo's egg",
   "Points": 5
 }
```
```json
{
   "Title": "dirt-cheap",
   "Description": "How much were student tickets for the 2019 BSides Charm security conference hosted in Baltimore?\n\nAnswer format: flag{value}",
   "Answer": "free",
   "Points": 5
 }
```
```json
{
   "Title": "founder",
   "Description": "What is the name of the person who created Linux?",
   "Answer": "Linus Torvalds",
   "Points": 5
 }
```
```json
{
   "Title": "Worm",
   "Description": "In 1998 a Cornell University graduate student was arrested for creating one of the first computer worms distributed through the Internet. This was the first felony conviction under the US 1986 Computer Fraud and Abuse Act. At the time, his father was head of the NSA. What was their last name? ",
   "Answer": ".*morris.*",
   "Points": 5
 }
```
```json
{
   "Title": "glitch in the matrix",
   "Description": "In the Matrix Reloaded Trinity uses Nmap to scan the network and then connects to a host using sshnuke. What IP address does she connect to?\n\nAnswer format is: flag{0.0.0.0}",
   "Answer": "10.2.2.2",
   "Points": 10
 }
```
```json
{
  "Title": "Sneakers",
   "Description": "What is the nickname of the character Dan Akroyd plays in the movie Sneakers?\n",
   "Answer": ".*mother.*",
   "Points": 10
 }
```
```json
{
   "Title": "Defaults",
   "Description": "A neighbor forgot the password for their D-Link DFL-300 router and have asked for you to gain access to it. They claimed that they never changed the password from when it was originally set up.\n\nWhat password should be tried first?",
   "Answer": "admin",
   "Points": 10
 }
```
```json
{
   "Title": "Your permanent record",
   "Description": "According to the Google website on Aug 23, 2001, how many web pages could you search?",
   "Answer": ".*1,?387,?529,?000.*",
   "Points": 30
 }
```
### Category: Web  
Browser inspect types of challenges.  

```json
{
   "Title": "Web",
   "Description": "[/web-challenge](/web-challenge)",
   "Answer": "I_lied_this_is_a_flag",
   "Points": 20
 }
```
```json
{
   "Title": "Logo hidden message #1",
   "Description": "The logo on the main has 3 hidden messages.\nCan you find the one that is visible to the eye?",
   "Answer": "unh wildcats",
   "Points": 20
 }
```
```json
{
   "Title": "Logo hidden message #2",
   "Description": "The logo on the main has 3 hidden messages.\nFind you can the one visible to a command line?",
   "Answer": "flag{service over self}",
   "Points": 20
 }
```
```json
{
   "Title": "Logo hidden message #3",
   "Description": "The logo on the main has 3 hidden messages.\n\nCan you find the one hidden  in the \"Old Man\"?",
   "Answer": "live free and cyber",
   "Points": 20
 }
```
```json
{
   "Title": "Find the cave",
   "Description": "26.357896, 127.783809",
   "Answer": "batman",
   "Points": 30
 }
```
```json
{
   "Title": "Token appreciation",
   "Description": "JavaScript Object Signing and Encryption (JOSE) is a framework specifying ways to securely transmit information on the internet. It's most well-known for JSON Web Tokens (JWTs), which are used to authorise yourself on a website or application. JWTs typically do this by storing your \"login session\" in your browser after you have authenticated yourself by entering your username and password. In other words, the website gives you a JWT that contains your user ID, and can be presented to the site to prove who you are without logging in again. JWTs look like this:\n\neyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJmbGFnIjoiY3J5cHRve2p3dF9jb250ZW50c19jYW5fYmVfZWFzaWx5X3ZpZXdlZH0iLCJ1c2VyIjoiQ3J5cHRvIE1jSGFjayIsImV4cCI6MjAwNTAzMzQ5M30.shKSmZfgGVvd2OSB2CGezzJ3N6WAULo3w9zCl_T47KQ\n\nFlag format is crypto{...}",
   "Answer": "crypto{jwt_contents_can_be_easily_viewed}",
   "Points": 30
 }
```
```json
{
   "Title": "Buckets of fun",
   "Description": "Downloadable workbooks: https://spy-museum.s3.amazonaws.com/ \nFetch the name of last modified public file, it will indicate a compromise.\n\nThe flag is the name of the file.\n",
   "Answer": "208b605c01bc1fd2b9ad92a96f77a169a84643cdeb82a9e64204e23f501afa17371012ec4c2928fda5477f19eaecf9ff449e2accaef00c2d842bf9654e48a232.txt",
   "Points": 40
 }
```

### Questions/Concerns/Suggestions/Bugs
Please post issues to the [GitHub page](https://github/kengraf/GenCyber)
