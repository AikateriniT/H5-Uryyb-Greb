Uryyb Greb

Choose a password manager. Explain: (This subtask y does not require tests with a computer if the question can be answered without them)


    - What treaths does it protect against?

A password manager provides protection from many types of attacks, theoretically any password manager is vulnerable to attacks, BUT the data that is stored there is encrypted so no one is able to read it even the company who built the password manager itself. 

Some of my personal favourites are KeePassXC and LastPass since they are using military-grade AES-256 encryption which means that no one can read the information stored in your account. Both of them are using a master password, which is the key to decrypt all stored information, that is only known to the user. In case the user forgets this password all information is trashed. 
So, this way the user is protected from two serious threats. One of them is a data leak that either a hacker or the developing company itself might try to sell online for money, and second from a malware that will try to retrieve the information from your computer. 

By utilizing a good password manager also helps out to create random strong passwords with a password generator, so the user is safe from password spraying (dictionary attacks).

Password managers are also convienient for those who have a weak memory. They can ensure that they will never forget their passwords, no matter how complex they are. 

Another threat that you are protected from is the weak or re-used passwords, both KeePassXC and LastPass are using a password audit that gives a warning of weak or re-used passwords.

Two big threats that a password manager DOES NOT protect you from though is: 

  - from a man-in-the-middle attack when the user decides to connect to the internet from a public network. 
  - from a malware that logs the users keystrokes. It is the user's responsibility to keep their computer malware free. 

Password managers are the safest way to store sensitive data, but we must remember that the user also is responsible for his data. His actions must comply with the general online safety rules, such as do not share sensitive information with unknown sites(phishing, low security websites), do not write your passwords through links that come as emails (phishing), do not download software from unknown sources (malware, virus, ransomware) etc. 

    - What information is encrypted, what's not?
    
With KeePassXC and LastPass, all information inside the file is encrypted. 

    - What's the license? How would you describe license's effects or categorize it?
    
GNU General Public License Version 3. The KeePassXC is an open source program thus it is free. 

    - Where is the data stored? If in "the cloud", which country / juristiction / 
    which companies? If on local disk, where?
    
The passwords/data is stored on the local disk at a folder of the user's choice. A file with the extention .kdbx, is created which requires a master password in order to access it. In addition, this type of PM allow the user to store the file on the cloud of their preference and gain access to it from multiple devices. It is a decentralized service, so the user has the freedom of choice where to store their file. 

It saves many different types of information, such as usernames, passwords, URLs, attachments, and notes in an offline, encrypted file that can be stored in any location, including private and public cloud solutions.

    - How is the data protected?

KeePassXC places controls over the access to this data so other applications cannot read it (unless they have administrative rights).

With these two password managers the encryption used is AES-256 The Advanced Encryption Standard (AES), also known by its original name Rijndael, is a specification for the encryption of electronic data established by the U.S. National Institute of Standards and Technology (NIST) in 2001.

The Advanced Encryption Standard (AES) is defined in each of:

FIPS PUB 197: Advanced Encryption Standard (AES)
ISO/IEC 18033-3: Block ciphers

For additional security steps:

Users can add Twofish or ChaCha20 encryption for an extra layer of security. It is also compatible with Yubikey (a USB multifactor authentication method) for supreme security of the KeePassXC database file. 

Demonstrate the use of a password manager.
-----------------------------------------------------------------------------------------------

I will demonstrate you the use of KeePassXC because this is the one that I am using and I am familiar with. 

The reason I prefer it, is because it has a clean and understandable interface and it is easy to use. 
________________________________________________________________________________________________

Let's start from the beginning though, with the first steps of installation and creating a new user. 

    - Step 1: Download KeePassXC application and create a new database.

https://keepassxc.org/download/
________________________________________________________________________________________________
Note!
Before installing KeePassXC, you should always verify that your download matches the signature that is published alongside the release package!

Warning: Please do not download unofficial packages from sources you don't trust!
________________________________________________________________________________________________
Open the KeePassXC app after you have successfully downloaded it and click create a new database. 
![1](https://user-images.githubusercontent.com/113516460/221530545-43786527-a930-4919-bbcc-b589f805d1f3.JPG)

After this the database generator wizard appear and you have to name your new database.

![2](https://user-images.githubusercontent.com/113516460/221530973-f7796f6e-deef-4cda-9715-5904fcd46a2d.JPG)








