# UNH GenCyber : Tuesday “A history of secrets” Lesson Plan
"A history of secrets" covers fundamental cipher operations to current everyday use of cryptography.

## Lesson Description
A "Cipher History" module introduces transposition and substitution as fundamental cipher operations. A second module "Modern Cipher" demonstrates how cryptography is used now in our daily lives.

### Prerequisite Knowledge
Students should have a basic understanding of how to use a web browser and be able to engage using remote meeting tools.

### Length of Completion
The lesson has two (2) modules each containing a set of lessons. Each lesson starts with a brief (15 minute) overview to provide context, instructions, and goals for the students.  Students are then a hands-on exercise that is typically completed in 10-30 minutes.  The modules and lessons have the following sequence.  

*"Cipher History" module*
Lesson: Transposition.  The hands-on exercises uses the Greek/Sparta Scytale cipher
Lesson: Substitution.		The hands-on exercises uses the Caesar cipher.
Lesson: Frequency Analysis. 	The hands-on exercises uses Civil War messages encoded with the Vigenère cipher.
Lesson: Compound.		The hands-on exercises uses the Pringle can Enigma exercise.

*"Modern Cryptography" module*

Lesson: Symmetric block cipher. The hands-on exercises uses the Data Encryption Standard (DES).
Lesson: Asymmetric cipher. The hands-on exercises uses the RSA algorithm.

## Applicable First Principles and Concepts

### GenCyber First Principles
<table border="0">
 <tr>
  <td><i>Abstraction</i></td>
   <td><i>Data Hiding</i></td>
   <td>Domain Separation</td>
   <td><i>Layering</i></td>
   <td><i>Least Privilege</i></td>
 </tr>
 <tr>
   <td>Minimization</td>
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
[Pringles Enigma lab](http://wiki.franklinheath.co.uk/index.php/Enigma/Paper_Enigma )  
[Cyber Chef](https://gchq.github.io/CyberChef/)  
[Spy Museum](https://www.spymuseum.org/)  


## Accommodations Needed
Special technical setup may be needed for students who are visually or physically impaired to use the
computer or engage in a remote meeting.

## LEARNING OUTCOMES
- Demonstrate an understanding of ciphers based on transpostion and substitution.
- Demonstrate the ability to use Internet resources to perform cipher operations.
- Demonstrate the use of frequency analysis to decode enciphered messages.

## LESSON DETAILS
### Assessment
The assessment for this lesson is a combination of informal observation and game statistics:  
- The number of students completing the base hands-on exercise for each lesson.  
- The number of students attempting or completing the bonus exercises.

### Differentiated Learning Opportunities
Hands-on exercise provides a base challenge and one or more bonus challenges.  
Online resources are provided for self-paced study.

## LESSON PREPARATION
### General
Review the "Pringles Can" videos to understand the "Cipher History" module's hands-on exercises  

*Scytale demonstration using a Pringles can*
[YouTube video](https://youtu.be/XBv6A2w3lz4)

*How to assemble a Pringles can Enigma machine*
[YouTube video](https://youtu.be/qemkHa7ozw4)

*Demonstration of Caesar, Vigenere, and Enigma*
[YouTube video](https://youtu.be/DHilx3lxoBo)  

*Asymmetric Encryption - Simply explained*
[YouTube video](https://www.youtube.com/watch?v=AQDCe585Lnc)  

*Feistel Cipher*
[Wikipedia](https://en.wikipedia.org/wiki/Feistel_cipher)

*DES*
[Wikipedia](https://en.wikipedia.org/wiki/Data_Encryption_Standard)

^AES*
[AES explained](https://www.youtube.com/watch?v=mlzxpkdXP58)

### SOFTWARE
This lesson uses only online based resources, no software installs are required.
## LESSON 
### Cipher History: Scytale Lesson
Points to be stressed during the lesson
- Transposition is just rearranging letters
- The transposition needs to be reversable, not random
- Easy to decode once the process is known
- Encrypted text has periods based on the circumference of the "rod"

Discussion: Would any of the following *tricks* make deciphering harder?
- Writing along the seams
- Spacing
- Font size
- Doubling/Tripling up letters
- Orientation of writing
- Very thin strip on a smaller "rod"

Instructions for hands on exercise
- Demonstrate the process
- Use your camp introduction story as the message
- Smaller letters and tighter spacing will allow a long message
- Allow 15 minutes

Bonus work: A second message for students that finish quickly
- Use the back of ribbon
- Using a different sized "rod"
- Use a difference writing style: spacing, seams, orientation

Wrap up
- Stress transposition
- Can you decipher the message without the Pringles can?
- Tonight ask a family member to try decrypting

### Cipher History: Caesar Lesson
Points to be stressed during the lesson
- Substitution, changing the values of the characters
- The process needs to be reversable
- The *key* is set once for the entire message
- Code wheels make the encrypting/decrypting process easier 

Discussion: Would any of the following *tricks* make deciphering harder?
- Encrypting only every other letter or words
- No spacing between words
- Adding a transposition 

Instructions for hands on exercise
- Assemble Pringles can (Order of rotors is critical)
- Allow 10 Minutes
- Demonstrate (Dog/Cat)
- Post message for the class to decrypt in chat: "Hashulhqfh lv wkh whdfkhu ri doo wklqjv"
- Remind that encrypted "D" is plain text "A"
- Allow 10 minutes
- Each student picks their own key, encrypt the name of their favorite movie and copy the encryption to their Discord channel
- Copy encrypted message into their channel
- Allow 10 minutes

Bonus work: A second message for students that finish quickly
- Use "Phq zloolqjob eholhyh zkdw wkhb zlvk"
- Encrypt a short message and copy to your Discord channel

Wrap up
- Stress substitution changes values in a reversable manner
- Analyzing words and letter groups can discover the key 

### Cipher History: Vigenere Lesson
Points to be stressed during the lesson
- A "keyed" substitution cipher
- The Caesar cipher with the offset changing for every letter
- Considered unbreakable until mid 1800's
- Short keywords lead to repetition in the cipher text  
- Guess a plain text word you can determine part of the key phrase

Discussion: Civil War messages broken
- Many messages using an agreed upon key phrase
- Words were often purposely misspelled, partial, or phonetic

Instructions for hands on exercise: 
- Decrypt: "UNIEK- CXNKVNED JJTRRK- ISLX- KFYHJEER-"
- Here’s how to crack this code–we will start you out with the first two letters then you do the rest: 
1. Set Ring I.  The "A" on Input/Output rotor should match the first letter in your key word, which is the letter M or (period 1).
2. On Ring I find the first letter in your enciphered message (the letter U)
3.  Read the letter on Input/Output: (the letter I)
4. Repeat steps 1-3.  2nd letter of key with 2nd letter of cypher.  FYI: whenever there is an "A" in the key the cypher text and plain text are the same!  After using the last letter in the key go back to the 1st in the key continue until you run out of cipher text.
It might help to make a table or spreadsheet to keep things organized.  

| Key |	M	| A	| N	| E	| H	| E	| S	| T	| A	| R	| B	| L	| U	| F	| F	| M	| A	| N	| E	| H	| E	| S	| T |  
| ----- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |   
| Cipher | U | N | I | E | K |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  
| Plain | I | N |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  

- What to do with the hyphens?  Decoding hyphens can be tricky.
- Hyphens are sometimes used as a placeholder for a letter that the reader could just guess.
- Sometimes a hyphen is used to throw off the letter count for anyone trying to break the cipher.
- Simple rule: If you have a complete word when you get to the hyphen in the cipher, just ignore the hyphen.  If the hyphen is needed to complete the word, skip the current key letter and fill in the word with your guess.

Allow 30 minutes

Bonus work: A second message for students that finish quickly
- Bonus messages: From Jefferson Davis 11 April, 1865  Code: "COME RETRIBUTION"
A scout reports that Genl Lee uidvvswvzfx mqs egaziox hw pjm tzat near to appomattox Courthouse yesterday. 
- Second bonus example: [Vicksburg Secret](https://owlcation.com/humanities/1863-Siege-of-Vicksburg-Secret-Message-Decoded)

Wrap up
- Short and reused keywords lead to compromise
- Military operations use a limited vocabulary 
- Transmission of random letters via telegraph(morse code) is error prone


### Cipher History: Enigma Lesson
Points to be stressed during the lesson
- Used by Germans in WWII
- Commercial SWISS design: 3 rotors, 1 reflector, key rings, plug board
- One or more rotors are shifted for every letter
- Reflector allowed two identically configured machines to both encrypt and decrypt
- New rotor configuration everyday
![image](https://user-images.githubusercontent.com/826579/118291434-9c4fa180-b4a5-11eb-896b-2137cfdea611.png)

Discussion: What made breaking Enigma hard?
- Known design
- Known rotor and reflector wiring
- How do you safely send the daily machine configuration?

Instructions for hands on exercise
- Demonstrate
- *Basic* rotors set to A B C allow 10 minutes
 - A E F A E  J X X B N  X Y J T Y
 - Hint: One word beginning with ‘C’
 - Answer: congratulations
- *Rotor turnover* rotors set to A B R allow 10 minutes
 - M A B E  K G Z X S G
 - Hint: Two words (4,6) beginning with ‘T’ and ‘M’
 - Answer: turn middle
- *Double stepping* rotors set to A D S allow 10 minutes
 - R Z F O G  F Y H P L
 - Hint: Two words (5,5) both beginning with ‘T’
 - Answer: turns three
 - ![image](https://user-images.githubusercontent.com/826579/118293609-d0c45d00-b4a7-11eb-9e5d-cbef1e014b86.png)

Bonus work: A second message for students that finish quickly
- [Review the BOMBE](https://www.britannica.com/topic/Ultra-Allied-intelligence-project#ref1073435)
- [Review Wiki](http://wiki.franklinheath.co.uk/index.php/Enigma)

### Modern Cipher: Symmetric Block Cipher Lesson

Points to be stressed during the lesson
- Plaintext and ciphertext consist of *fixed-sized* blocks
- The encryption/decrpytion includes many rounds (loop)
- Every round iterates a *Round Function* to transform plantext to ciphertext
- The key and output of previous round are the input to the round function
- Feistel cipher is a design pattern for block cipher
- The encryption and decryption in Feistel cipher
- DES block length, key length, rounds
- DES Expend, S-box, P-box
- Block cipher notation

Discussion:
- Does Feistel cipher always correctly decrypt the ciphertext?
- What is a good round function?

Instructions for hands on exercise
- Calculate L2 and R2 given the following round function
  1. F = R(i-1)
  2. F = R(i-1) xor K(i)
- Use CyberChef to do DES encryption and decryption

### Modern Cipher: Asymmetric Key Cipher Lesson

Points to be stressed during the lesson
- Asymmetric key cipher has two different keys for encryption and decryption
- The design is based on one-way function
- RSA algorithm procedure

Discussion:
- Why breaking RSA is difficult?
- Why factoring a large integer is difficult?

Instructions for hands on exercise
- Give p = 5 and q = 11, calculate the public and private key
- Show the encryption and decryption procedure

### Questions/Concerns/Suggestions/Bugs
Please post issues to the [GitHub page](https://github/kengraf/GenCyber)
