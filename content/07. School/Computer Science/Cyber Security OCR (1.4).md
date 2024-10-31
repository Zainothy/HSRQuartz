---
Topic: Computer Science GCSE
tags:
  - School
  - Networking
  - Computer-Science
Completed: 
Links:
  - "[[Networking (OCR) 1.3]]"
aliases:
  - CS
  - Security
  - "1.4"
---
# Fundamentals of Cybersecurity:

## Things that Threaten a Network:

### Hackers:


>[!info] Hacker
>👩🏻‍💻 **“Hacker”- User who gains or attempts to gain access computer system without authorisation, whilst intending to cause damage**

>[!info] Ethical Hacker 
>👨🏻‍💻 **“Ethical Hacker”- Experts in the security of computers who try to gain access to systems in order to find issues/vulnerabilities, if done with permission of the network owner/admin: it can be considered [Penetration Testing](https://www.cloudflare.com/en-gb/learning/security/glossary/what-is-penetration-testing/). If this is done without permission, it falls under the same definition of Hacker and is illegal Under the [Computer Misuse act](https://en.wikipedia.org/wiki/Computer_Misuse_Act_1990)** 


### Data Interception and Theft:

In networks, signals flow over hardwire or through radio waves. If someone gains access to said signals, they can intercept the data that they carry. This is difficult to do so on a wired network, as it will typically require access to the building, however it is much easier to gain access to a wireless network if you are close enough. This is why [Data Encryption on wireless networks](https://www.wi-fi.org/discover-wi-fi/security) is essential

There are different types of attacks on a wireless network: 

[A Man-in-the middle attack](https://en.wikipedia.org/wiki/Man-in-the-middle_attack) describes an attack where a hacker takes control of the connection between two people and intercepts the data that is passed between them. The hacker can take the data and alter it so that the recipient receives tampered data. 

## Denial of Service (DoS):

>[!info] Servers
>“Server”- A computer that provides 
 client computers with services, such as 
 a webserver hosting the Steam website, 
 servers are typically kept on 24/7: 
 Constantly listening for requests.

Severs are setup to be able to cope with a certain amount of size in traffic. In a DoS attack, a server receives an overwhelming amount of traffic beyond its capacity. As a result, other users attempting to access the server may find their requests unprocessed, leading to an inevitable service denial.

A great example of DoS attack is the Amazon Web Services attack from February 2020. They reached a peak traffic volume of 2.3Tbps, for reference: that is 2,300,000,000,000 bits every second.

## Distributed Denial of Service (DDoS): 

In a DDoS attack, the attack originates from a distributed network of computers, typically a [Botnet](https://www.cloudflare.com/en-gb/learning/ddos/what-is-a-ddos-botnet/). The term botnet is short for bot network and is a computer network that is being controlled by a single operator. The operator can command the computers to do something in unison, such as flood a server with requests.

## SQL Injection: 

> [!info] Injection
>**“SQL Injection”- Technique used by a person with malicious intent to manipulate an SQL statement to their benefit.**

>[!info] SQL 
>**“[SQL](https://en.wikipedia.org/wiki/SQL)”- Structured Query Language, used to form queries to extract or manipulate info in a Database.**

Imagine a website that requires you to enter some login information, username + password. The parameters that you enter are then sent to the web server, this is then used to execute a SQL Query against the database to look for your details. If they are found, and the details are correct: you gain access.

The SQL query injects the data that you entered. If the code that sets up the query is not well written, it can be exploited to enter more information than asked for and then incorporated when the query is run. If this extra code bypasses the sign in system, the malicious user can log in.

SQL Injections can also:

- Extract Data, eg. credit card lists
- Delete Data
- Update Data
- Insert data
- Execute commands to install malware

This can often be avoided with well-written code, such as input validation that returns a rejection when inputs contain unexpected content. A "Parameterised Statement" ensures the query string and parameter values are transmitted separately, ensuring their safe and secure handling.

## Password Attacks:
---
>[!info] Password Attack 
>**One of the ways used to access ones password. There are Brute Force attacks and Dictionary attacks**

### Brute Force:

This type of attack makes use of a computer program that constantly attempts all sorts of character combinations, until it finds the correct one.

If the password is short and simple, made up from a small character selection. It will be easy to crack. Example: If your password was all lower case, there are 6^26 possibilities. A computer could sequence these in seconds, with enough power.

If the Pswd was 32 chars long and:

- All 26 lower case characters
- All 26 Upper Case used
- All of the digits
- ten special characters

the possibilities would be:

### Dictionary Attack: 

> [!info] Dictionary Attack
> **Brute force attack that uses password lists (dictionary) to check if the password that is being cracked, matches the one in the list.**
This list may include common passwords and passwords that have been leaked from external sources. Each password in the dictionary is attempted until the correct one is found.

Using the same Password for multiple sites is also a security risk, as if a data breach occurs and private info is leaked on the dark web. The password you use for virtually everything, may have just been leaked.

## Impact of Network Security failure:

If a system is compromised or victim of an attack, there can be significant damage done.

- If commercial data is stolen/ accessed, it can be sold and/or redistributed
- Typically, when personal data is stolen: the organization will be investigated and likely fined.

Often, reputational damage is more significant: it can damage a user’s trust in an organization or cause stakeholders to reconsider their assets in the company. This can reduce traffic and/or result in loss of revenue. 

## Footprinting: 

> [!info] Footprinting
> **The process of gathering info around systems prior to an attack, e.g: finding out the OS used or what vulnerabilities the service may have.**


The attacker may look for information around users, such as finding the email addresses of a few of the orgs workers. As it could be used to guess how UserID is structured. Info from social media can also be manipulated.

## IP Spoofing: 


> [!info] IP Adress 
> **A unique address for a computer on a network that uses the internet & its protocols. These networks may exchange data in the form of packets, these packets will have the senders IP address on the header. Many networks have firewalls that only allow packets to be received from trusted IP addresses.**

A malicious user can use software to alter a packets source address to make it appear that the packet came from a trusted source- this is known as [IP Spoofing](https://www.cloudflare.com/en-gb/learning/ddos/glossary/ip-spoofing/) . This can allow the user to to carry out things such as:

- Adding you computer to a botnet, that carries out large scale Cyber Attacks
- Infecting your device with malware
- Circumventing an Authentication system:
    - Example: SSO, an authentication scheme that allows users to log into organisation software systems with a single set of login details. Spoofing IP addresses can allow an attacker to access computers on the same network without authentication.

# Controlling Access to Networks: 

### Two Factor Authentication (2FA):

Passwords are not 100% safe, so nowadays many systems require 2FA. Meaning, another piece of evidence is required in order to verify a login, an example being a verification code sent to an email, phone number or authentication app. It could also be a personal question that you setup

There is a wide range of 2FA systems, banks used small keypads that are sent out customers. Many modern systems now use 3rd party authentication apps such as google authenticator to generate 2FA codes.

## Biometric Authentication:


> [!info] Biometric
> **A physical characteristic, e.g Fingerprint, that can be used to identify who you are. Biometrics have become more common as tech like iris scanners and fingerprint readers improve.**

Fingerprint is often used to access phones, apps and authorise payments. Some Airports have started using iris recognition as part of their security

An experimental/emerging biometric tech is Voice Recognition, as our voices are unique. Many banks have started to uses Voice Recognition for authentication.

## Biometric Spoofing


> [!info] Biometric Spoofing
> **A term used to describe the methods used for fooling biometric authentication systems/ scanners. Fingerprints can be damaged by cuts, and can be spoofed quite easily as copies are easy to get a hold of. Iris authentication is one of the most secure, as the iris is protected by the cornea**

