# UNH GenCyber : Tuesday “A history of secrets” Lesson Plan
"A history of secrets" covers fundamental cipher operations to current everyday use of cryptography.

## Lesson Description
A "Cipher History" module introduces transposition and subsitiution as fundamental cipher operations. A second module "Modern Cipher" demonstrates how cryptography is used now in our daily lives.

### Prerequisite Knowledge
Students should have a basic understanding of how to use a web browser and be able to engage using remote meeting tools.

### Length of Completion
The lesson has two (2) modules each containing a set of lessons. Each lesson starts with a brief (15 minute) overview to provide context, instructions, and goals for the students.  Students are then a hands-on exercise that is typically completed in 10-30 minutes.  The modules and lessons have the following sequence.  

*"Cipher History" module*
Lesson: Transposition.  The hands-on exercies uses the Greek/Sparta Scytale cipher
Lesson: Substitution.		The hands-on exercies uses the Caesar cipher.
Lesson: Frequency Analysis. 	The hands-on exercies uses Civil War messages encoded with the Vigenère cipher.
Lesson: Compound.		The hands-on exercies uses the Pringle can Enigma exercise.
*"Modern Cryptography" module*
## DX:TBD lesson titles

lesson (AES, RSA) 

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
## DX:TBD related links

## Accommodations Needed
Special technical setup may be needed for students who are visually or physically impaired to use the
computer or engage in a remote meeting.

## LEARNING OUTCOMES
- Demonstrate an understanding of ciphers based on transposiotn and subsitution.
- Demonstrate the ability to use Internet resources to perform cipher operations.
- Demonstrate the use of frequency analysis to decode enciphered messages.

## LESSON DETAILS
### Assessment
The assessment for this lesson is a combination of informal observation and game statistics:  
- The number of students completing the base hands-on exercise for each lesson.  
- The number of students attempting or completing the bonus exercises.

### Differentiated Learning Opportunities
Hands-on exercise provide a base challenge and one or more bonus challenges.  
Online resources are provided for self paced study.

## LESSON PREPARATION
### General
Review the "Pringles Can" videos to understand the "Cipher History" module's hands-on exercises  

*Scytale demonstration using a Pringles can*
[YouTube video](https://youtu.be/XBv6A2w3lz4)

*How to assemble a Pringles can Enigma machine*
[YouTube video](https://youtu.be/qemkHa7ozw4)

*Demonstration of Caesar, Vigenere, and Enigma*
[YouTube video](https://youtu.be/DHilx3lxoBo)  

Review/Personalize the lecture [Link to lesson slides](images/CipherHistory-LectureSlides.pdf)
## DX:TBD related content

### SOFTWARE TBD
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
- Demostrate the process
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
- Subsitution, changing the values of the characters
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
- Demostrate (Dog/Cat)
- Post message for the class to decrypt in chat: "Hashulhqfh lv wkh whdfkhu ri doo wklqjv"
- Remind that encrypted "D" is plain text "A"
- Allow 10 minutes
- Each student picks thier own key, encrypt the name of their favorite movie and copy the encryption to their Discord channel
- Copy encrypted message into their channel
- Allow 10 minutes

Bonus work: A second message for students that finish quickly
- Use "Phq zloolqjob eholhyh zkdw wkhb zlvk"
- Encrypt a short message and copy to your Discord channel

Wrap up
- Stress subsitution changes values in a reversable manner
- Analyzing words and letter groups can decover the key 

### Cipher History: Vigenere Lesson
Points to be stressed during the lesson
- A "keyed" subsitution cipher
- The Caesar cipher with the offset changing for every letter
- Considered unbreakable until mid 1800's
- Short keywords lead to repetition in the cipher text  
- Guess a plain text word you can determine part of the key phrase

Discussion: Civil War messages
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
| Key   |	M	| A	| N	| E	| H	| E	| S	| T	| A	| R	| B	| L	| U	| F	| F	| M	| A	| N	| E	| H	| E	| S	| T |  
| ----- | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - |   
| Cipher | U | N | I | E | K | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - |  
| Plain | I | N | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - |  

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
- Transmission of random letters via telegraph is error prone


### Cipher History: Enigma Lesson
Points to be stressed during the lesson
- A "keyed" subsitution cipher
- The Caesar cipher with the offset changing for every letter
- Considered unbreakable until mid 1800's
- Short keywords lead to repetition in the cipher text

Discussion: Would any of the following *tricks* make deciphering harder?
- Writing 

Instructions for hands on exercise
- Demostrate
- Allow 15 minutes

Bonus work: A second message for students that finish quickly
- Use 

Wrap up
- Stress 


## DX:TBD lessons detail

### Questions/Concerns/Suggestions/Bugs
Please post issues to the [GitHub page](https://github/kengraf/GenCyber)
