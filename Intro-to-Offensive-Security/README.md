# Intro to Offensive Security

## Overview
### Objective:
We are hacking a bank!! Transferring heaps of money from other people's account to our own bank account 😈

### Tool(s):
* [**GoBuster**](https://www.kali.org/tools/gobuster/)
  > official definition: a tool used to brute-force URIs including directories and files as well as DNS subdomains. <br>
  > my definition: enumerate directories / DNS subdomains from a URI.

## Procedure

### Task 1 - Hacking your first machine
#### To Do
1. Click the terminal icon.
![image](https://user-images.githubusercontent.com/66156414/184582304-bf621e74-b7f8-4f62-b5b8-3390a506a390.png)
2. You will then see an open terminal.
![image](https://user-images.githubusercontent.com/66156414/184582363-3f76d890-d897-489c-978a-cdca69c6425e.png)
3. In the terminal, type `gobuster -u http://fakebank.com -w wordlist.txt dir`.<br><br>
    > command desc:
    > - -u (string) --> string: the target URL or Domain
    > - -w (path) --> string: path to the wordlist
    > - dir --> uses directory/file enumeration mode
4. Notice the directory name `/bank-transfer`.
![image](https://user-images.githubusercontent.com/66156414/184583678-29881491-6c35-460b-ac13-9d69e1bdc357.png)
5. Type `http://fakebank.com/bank-transfer` in the search engine and BOOM! You found the secret bank transfer page!
![image](https://user-images.githubusercontent.com/66156414/184583888-a7c8ae26-4bd5-41f0-b881-dd2d04ddcc26.png)
6. Now let's transfer some money to your account!! From acc 2276 to 8881, with the amount of $2000.
![image](https://user-images.githubusercontent.com/66156414/184584013-4b462efd-52c9-4cfe-9598-a51d469e5ae9.png)
7. Look who's rich now 😎
![image](https://user-images.githubusercontent.com/66156414/184584086-10f9210c-877d-4109-a310-028c1f41126f.png)

#### Answers
1. When you've transferred money to your account, go back to your bank account page. What is the answer shown on your bank balance page?
    > `BANK-HACKED`

### Task 2 - What is Offensive Security?
Offensive security
- The process of:
  - breaking into computer systems
  - exploiting software bugs
  - finding loopholes in applications
- Goal
  - gain unauthorized access to them.

Defensive security
- The process of:
  - protecting an organization's network and computer systems<br>
- How?
  - analyzing and securing any potential digital threats.
  - note: learn more in the digital forensics room.
- Goal
  - understand how a device was hacked.
  - track down cybercriminals.
  - monitoring infratructure for malicious activities.

### Task 3 - Careers in cyber security
Hackers: security consultants<br>
Defenders: security analysts fighting cybercrime
<br><br>
Career choices:
- Penetration Tester - Responsible for testing technology products for finding exploitable security vulnerabilities.
- Red Teamer - Plays the role of an adversary, attacking an organization and providing feedback from an enemy's perspective.
- Security Engineer - Design, monitor, and maintain security controls, networks, and systems to help prevent cyberattacks.
