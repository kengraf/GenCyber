# UNH GenCyber : Monday "Hello World!" Lesson Plan
# Modules: Introductions, Social Engineering, and Bug Bounty Hunting

## Lesson Description
As this is their first day together, students will learn about follow classmates through the exchange of personal stories.  Students will preform research and reconnaissance, the Open Source Intelligence Gathering (OSINT), activities required for effective social engineering.  Students will discover a variety of client- and server-side bugs and automatically get rewarded with GenCyberCoins for those. Some bug examples: sensitive data exposure, broken authentication, XSS, user input validation, and local file inclusion.
### Prerequisite Knowledge
Students should have a basic understanding of how to use a web browser and be able to engage using remote meeting tools.

### Schedule
The lessons has three (3) modules. Each module starts with a brief (15 minute) overview to provide context, instructions, and goals for the students.  Student typically complete each module in 90-120 minutes.  The modules have the following sequence.  
Module 1: Introductions  
 All students and instructors take three (3) minutes to present thier personal story to the class.  The story can be an event, place, or emotion the student would like to share. The story is meant to be an ice-breaker, it is used in the next module, and again in lessons later in the week.  
 Module 2: Social Engineering  
 This module uses the reconnaissance features of GenCyberCoin.  For each student story, instructors will post a single question.  Students receive points (coins) for each correct answer.  The questions will require a small amount of research time (less than 5 minutes).  Instructors may post additional group questions to foster additional student exchanges.
 Module 3: Bug Bounty Hunting 
 This module uses a series of programming flaws built into GenCyberCoin. The game provides a list of bugs to locate, with hints.  The listed is roughly ordered by difficulty.  Coins are rewarded for each bug successfully located.  Students work at their own pace, are encouraged to collaborate on methods, and not required to complete all tasks.
### Level of Instruction
The lesson is intended for high school learners (beginner and intermediate levels)

## Applicable First Principles and Concepts

### GenCyber First Principles
<table border="0">
 <tr>
  <td><b>Abstraction</b></td>
   <td><b>Data Hiding</b></td>
   <td>Domain Separation</td>
   <td><b>Layering</b></td>
   <td><b>Least Privilege</b></td>
 </tr>
 <tr>
   <td>Minimization</td>
   <td><b>Modularity</b></td>
   <td>Process Isolation</td>
   <td><b>Encapsulation</b></td>
  <td><b>Simplicity</b></td>
 </tr>
</table>
### GenCyber Cybersecurity Concepts
<table border="0">
 <tr>
  <td>Availability</td>
  <td><b>Confidentiality</b></td>
  <td><b>Defense in Depth</b></td>
 </tr>
 <tr>
  <td><b>Integrity</b></td>
  <td><b>Keep it Simple</b></td>
  <td><b>Think like an Adversary</b></td>
 </tr>
</table>
 
## Resources & Requirements
- Before the beginning of the lesson.  Each student needs to provide a personal story about an event in their life.  It can be an event, place, or emotion you would like to share.  It is meant to be brief less than 100 words, but must contain at least twenty words six characters or longer.  The last requirement is for lessons later in the week.
- Each student needs access to a browser and connected to the remote meeting both with both video and audio.
- Websites/Software used  
 - [GenCyberCoin Game](https://github.com/vitalyford/gencybercoin)
 - [Hacksplaining](https://hacksplaining.com)

### Accommodations Needed
Special technical setup may be needed for students who are visually or physically impaired to use the
computer.

## LESSON LEARNING OUTCOMES
- Demonstrate the ability to think like an adversary and identify what can go wrong on a website
- Demonstrate the ability to use Internet resources to gather relavent information during a reconnaissance effort.
- Learn about different types of vulnerabilities that are typical for websites.
- Learn the basics of web ethical hacking and exploitation.

## LESSON DETAILS
### Assessment
The assessment for this lesson is a combination of observation and statistics of the
following:
- The number of students answering the Reconnaissance questions correctly (the OSINT Ninjas
page).
- The results of the Bug Bounty activity (the Hall of Fame page).
### Extension Activities on the Hacksplaing site
- Learn about additional web attacks.
### Extension Activities on the GenCyberCoin platform
- Learn about password strength, where to check if the email and password have been
compromised, and how to correctly manage it.
- Learn about digital currency.
- Learn about blockchain and its applications beyond cryptocurrency.
### Differentiated Learning Opportunities
Advanced students can learn more attacks and find more bugs within the allocated time and learn more by exploring the links
that are related to the found bugs. Also, advanced students can discover more sophisticated search
queries by spending more time reading the material provided in the Reconnaissance activity.
## LESSON DELIVERY
### Instructor and Teaching Assitant Preparation
- Introductions
 - Validate all students have posted their personal story prior to the start of lesson
- Hacksplaining
 - Review lessons on [Hacksplaining](https://hacksplaining.com)
- GenCyberCoin
 - The instructor can learn how the GenCyberCoin platform works by watching a [12-minute video](https://github.com/vitalyford/gencybercoin).  
 - The **instructor** needs to follow the directions for deploying on Heroku.  
 - After the system is deployed, login in with “gcsuperuser/gcsuperuser” credentials, change the password.
 - Generate registration code for (admins), normally the instructor and all teaching assitants
 - Add recon questions based on student stories.
 - Add items to marketplace
 - Create new badges and activity information.
### Module 1: Introductions  
- All students and instructors take three (3) minutes to present thier personal story to the class.
### Module 2: Social Engineering  
- The instructor shows a [2-minute video](https://github.com/vitalyford/gencybercoin) about the GenCyberCoin platform to the students.
- Students navigate to the shared URL and register with the shared registration code.
- Students navigate to Features → Reconnaissance to learn about Open Source Intelligence Gathering (OSINT) and Social Engineering.
- Students answer as many questions as they can on the Reconnaissance page.
- Everybody can see everyone’s progress on the OSINT Ninjas page.
 Module 3: Bug Bounty Hunting 
 This module uses a series of programming flaws built into GenCyberCoin. The game provides a list of bugs to locate, with hints.  The listed is roughly ordered by difficulty.  Coins are rewarded for each bug successfully located.  Students work at their own pace, are encouraged to collaborate on methods, and not required to complete all tasks.
Student information

## Lesson walthrough
- Validate student story is posted and visible to classmates.
- Register an account and explore the GenCyberCoin platform.
2. Navigate to Features → Bug Bounty to learn about what kinds of bugs to search for on the
platform. There are hints in place to help you find those bugs.
5. Find as many bugs as you can on the Bug Bounty page. Everybody can see everyone’s progress
on the Hall of Fame page.
6. As you progress through the activities, you automatically earn GenCyberCoins and every
action/transaction is tracked on the Blockchain (Features → Blockchain).
7. Discuss the details of Reconnaissance and Bug Bounty as well as their implications in the real
world.
### Questions/Concerns/Suggestions/Bugs
Please post issues to the [Github page](https://github/kengraf/GenCyber)
