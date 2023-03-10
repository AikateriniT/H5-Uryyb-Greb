Uryyb Greb - Fifth homework
---------------------------------------------------------------------------------------------

Read and summarize (This subtask x does not require tests with a computer. Some bullets per article is enough for your summary, feel free to write more if you like)
€ Schneier 2015: Applied Cryptography: 10. Using Algorigthms: 10.1, 10.2, 10.3, 10.4 (from start until the start of "Dereferencing Keys" in 10.4)
---------------------------------------------------------------------------------------------

Chapter 10: USING ALGORITHMS

10.1 
Correct choice of algorithms:

    - Published algorithms, are a good choice in case they haven't been scrutinized yet.
    - Manufacturer's algorithms, are also a good choice since a manufacturer has a good reputation 
    and will not risk the good name of the entire company with weak algorithms.
    - Private consultants, offer options of reliable algorithms since they are best equipped to provide
    different algorithms.
    - Governement, is another option since they always opt for citizens' good.
    - Private initiative, means that each one can write their own algorithms based on the belief that 
    one can write his own, as long as they have cryptographic abilities.
    
These options have several issues, even though they look like they are suitable for different occassions. The outcome of this study is that no one should trust only one source, when it comes to security. Many "security consultants", are not familiar with very important terms of security and mainly about encryption. NSA at the moment has some of the biggest talents on encryption, but they are very secretive. 

Public algorithms analyzed in this book have both possitive and negative results. Military security organizations are cryptanalyzing, and they are not interested to publish their results. Public algorithms are safer though than any other algorithm implemented in secret environments. 

The question comes to, what algorithms NSA can break? 

In the sphere of secrecy, none organization incl. FBI will not introduce the how-to of DES-encryption. The how-to is of -ten times bigger secret than the information stored in a hard-drive for example. The only way to make NSA admit their ability to break algorithms is to encrypt something extremely valuable, leading to public admission of decryption. 

NSA like any other organization has limited resources. Meaning, they must choose wisely their targets. An assumption made here is that they prefer to solve their problems physically than in the digital world. 

ALGORITHMS FOR EXPORT

All algorithms exported from the US must be approved by the government. The assumption here is that all algorithms exported they have to been first broken by the NSA. Rumors about exported algorithms include:

    - Leak a key bit once in a while, embedded in the ciphertext.
    - “Dumb down” the effective key to something in the 30-bit range.
    - Use a fixed IV, or encrypt a fixed header at the beginning of each encrypted message.
    - Generate a few random bytes, encrypt them with the key, and then put both the plaintext and 
    the ciphertext of those random bytes at the beginning of the encrypted message. 
    
PUBLIC-KEY CRYPTOGRAPHY VERSUS SYMMETRIC CRYPTOGRAPHY

Public-key cryptography or symmetric cryptography?

Utility of public algoritmhs is a continuous debate since the cryptography was invented. Needham and Schroeder camy to the conclusion that the number and length of messages are greater with public-key algorithms than the symmetric algorithms. The symmetric algorithm was more efficient than the public-key algorithm. 

According to Whitfield Diffie:

Public-key cryptography is a new form of cryptosystem. The critisism of this system here is based both on security and performance. In comparison of the RSA and the DES system, the RSA was far more sufficient in terms of performance and DES required bigger keys. The need to build hybrid systems emerged. Public-key cryptography and symmetric cryptography are two completely different things. 

    - Symmetric cryptography is best for encrypting data. It is orders of magnitude faster and is 
    not susceptible to chosen-ciphertext attacks. It is best for key management and a myriad of protocols.
    
10.3 ENCRYPTING COMMUNICATIONS CHANNELS

Let's see a bit in practical terms how to encrypt messages. Theoretically encryption can happen at any layer of OSI communications model but practically it happens to the lowest layers or at the highest levels. 

There are two types of encryption depending on which layer it happens:

    Link-by-link encryption
When it happens at the lowest layers. All the information goes through a data link which is encrypted.  

    End-to-end encryption
When it happens at the highest layers. Data is encrypted selectively and remain encrypted until it reaches the recepient who is the only one with the ability to decrypt the message. 

LINK-BY-LINK ENCRYPTION

It is the easiest way to add encryption 
    

Choose a password manager. Explain: (This subtask y does not require tests with a computer if the question can be answered without them)
----------------------------------------------------------------------------------------------

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

KeePassXC places controls over the access to this data so other applications cannot read it (unless they have administrative rights). By default, KeePassXC prevents recordings and screenshots of the application window on Windows and macOS. This prevents inadvertent spillage of information during meetings and disallows other applications to capture the window contents.

With these two password managers the encryption used is AES-256 The Advanced Encryption Standard (AES), also known by its original name Rijndael, is a specification for the encryption of electronic data established by the U.S. National Institute of Standards and Technology (NIST) in 2001.

The Advanced Encryption Standard (AES) is defined in each of:

FIPS PUB 197: Advanced Encryption Standard (AES)
ISO/IEC 18033-3: Block ciphers

For additional security steps:

:shield: Users can add Twofish or ChaCha20 encryption for an extra layer of security. It is also compatible with Yubikey (a USB multifactor authentication method) for supreme security of the KeePassXC database file. 

Demonstrate the use of a password manager.
-----------------------------------------------------------------------------------------------

I will demonstrate you the use of KeePassXC because this is the one that I am using and I am familiar with. 

The reason I prefer it, is because it has a clean and understandable interface and it is easy to use. It is an application that supports all operating systems (windows, macOS, Linux) and it does not have a mobile app.  
________________________________________________________________________________________________

Let's start from the beginning though, with the first steps of installation and creating a new user. 

    - Step 1: Download KeePassXC application and create a new database.

https://keepassxc.org/download/
________________________________________________________________________________________________
Note ❗
Before installing KeePassXC, you should always verify that your download matches the signature that is published alongside the release package!

Warning ‼️ Please do not download unofficial packages from sources you don't trust!

Because KeePassXC does not allow to take screenshots for security reasons we must start the application with the --allow-screencapture command line flag.

________________________________________________________________________________________________
Open the KeePassXC app after you have successfully downloaded it and click create a new database. 
![1](https://user-images.githubusercontent.com/113516460/221530545-43786527-a930-4919-bbcc-b589f805d1f3.JPG)

After this the database generator wizard appear and you have to name your new database.

![2](https://user-images.githubusercontent.com/113516460/221530973-f7796f6e-deef-4cda-9715-5904fcd46a2d.JPG)

By clicking next, you will get encryption settings slide, and the developers actually do not recommend at this point to change anything except the decryption timer. By choosing bigger decryption time the security increases but the time to decrypt the passwords will be longer. 

![3](https://user-images.githubusercontent.com/113516460/221531398-16a97a9d-fd26-435c-9793-142632538829.JPG)

Then, you will get the tab where you have to create your master password, at this step you must be extra careful. By loosing the master password you will not be able to have access to you information never again. Keep this password for your database safe. Either memorize it or note it down somewhere.

![4](https://user-images.githubusercontent.com/113516460/221532732-2b9b8392-e091-4da6-89b9-1f7a0fbf5669.JPG)

Click Done and you will be asked to select the location that the database file will be stored. You can save the file wherever you wish. Even in the cloud of your preference in case you want to use this database across multiple devices. It is fully encrypted at all times so unuthorized access is prevented. 

    - Step 2: Storing and generating passwords.
    
Now that you are all set and have created your first database you are ready to store your passwords, usernames, URLs, or even important notes that have to be encrypted. You can store as many entries as you want. 

![5](https://user-images.githubusercontent.com/113516460/221534425-4a2ffa21-e563-47f7-a0d9-b8a7f4109a7d.JPG)

Let's start by checking a bit the homepage. 

    A) Database - Open database, Save database, Lock database.
    B) Entries - Create Entry, Edit Entry, Delete Selected Entries
    C) Entry Data - Copy Username, Copy Password, Copy URL, Perform Auto-Type
    D) Tools - Password Generator, Application Settings
    E) Search
    
The toolbar provides a quick way to perform common tasks with your database. The user also through the View tab can decide whether to use a dark or a light mode. 

To add a new entry: Navigate to Entries > New Entry (Or, press Ctrl+N). The following screen appears:

![7](https://user-images.githubusercontent.com/113516460/221537056-d5070e75-f00a-4153-9a92-01c306e1ac38.JPG)

    1️⃣ You have to add a title for your entry.
    2️⃣ Then the username
    3️⃣ Add the password, which can be chosen by you or can be generated by clicking the small square next to the 
    visible/invisible button.
    4️⃣ The URL. After you add a URL to an entry you can press the download button to automatically download the 
    website’s icon for this entry.
    5️⃣ Add tags if you wish 
    6️⃣ An expiration day, which means that the manager will ask you to change your password.
    7️⃣ Add notes for this website. 
    
Generate a random password with the password generator by clicking the small square buttton. 

![8](https://user-images.githubusercontent.com/113516460/221538384-43e63190-9034-4f56-8a69-de9c0d96af26.JPG)

From the choices 1,2,3,4 you can pick what kind of characters you want to be included to your password. Some websites do not allow all kinds of special characters for example. Then from number 5 you can choose how many characters long you want your password to be. The green bar under the password shows you how strong your password is. 

Using KeePassXC as an authenticator app by adding TOTP to an entry. 
__________________________________________________________________________________________
The KeePassXC database offers also the option to use it as an authenticator app, by adding a TOTP to an entry. It is exactly the same as Google Authenticator or any other authenticator.

Timed One-Time Passwords is a two-factor authentication method. These codes are typically six digits long and change every 30 seconds. They are derived from a shared secret value and the current time. Once set up, KeePassXC can calculate TOTP codes like any authenticator app, such as Google Authenticator. The codes can be used with copy/paste, browser extension, and Auto-Type.

***Note :exclamation: The computer must be synchronized with the internet time source in order to generate valid TOTP codes.***

***Warning :bangbang: It is wise to create one database for the passwords and another one for the TOTP codes. In this case the benefits of two-factor authentication will not be eliminated. The TOTP database is good to be unlocked only when needed.***

To add TOTP to a database entry, you must first retrieve the secret string from the website or application you are authenticating to. Often this secret is accompanied with a QR code and can be copy/pasted below. 

![9](https://user-images.githubusercontent.com/113516460/221542091-73879923-c602-4a2b-8fc8-97bc393959d3.JPG)

Once obtained, right-click the desired entry (1), choose TOTP → Set up TOTP…​ (2), and the setup dialog will appear. In that dialog, paste the secret code from the website (3), setup any custom settings (rare) (4), then press OK to save the settings.

![91](https://user-images.githubusercontent.com/113516460/221542414-cc53a722-00ea-4a68-8216-2317b4f6a54f.JPG)

After an entry is configured with TOTP, you will see a clock icon in that entry’s row and have the ability to reveal the current code in the preview pane. Additionally, you can navigate to the entry’s TOTP menu to show the code in a separate window. You can also view the secret and configuration as a QR code for exporting to a mobile device. TOTP codes can be entered into forms with the browser extension, with Auto-Type by using the {TOTP} placeholder, or via menu options in the Auto-Type selection dialog.

![912](https://user-images.githubusercontent.com/113516460/221542596-e0eb2dc7-b82e-4359-ba9a-5883424feb3c.JPG)

    - Step 3: Setup Browser integration.
    
The KeePassXC-Browser extension is installed within your web browser so that you can automatically pull usernames and passwords from KeePassXC and populate them directly into website fields. It is a very useful and secure extension that enhances your productivity while using KeePassXC. With this extension, you do not need to manually copy the data from your KeePassXC database and paste it into the website fields.

The KeePassXC-Browser extension is available on the following web browsers:

    Google Chrome, Vivaldi, and Brave
    Mozilla Firefox and Tor-Browser
    Microsoft Edge
    Chromium

You can download the KeePassXC-Browser extension from your web browser. To download the KeePassXC-Browser extension, perform the following steps:

Click the link corresponding to your browser:

[Chrome, Chromium, Vivaldi, and Brave](https://chrome.google.com/webstore/detail/keepassxc-browser/oboonakemofpalcgghocfoadofidjkkk)

[Mozilla Firefox and Tor-Browser](https://addons.mozilla.org/en-US/firefox/addon/keepassxc-browser/)

[Microsoft Edge](https://microsoftedge.microsoft.com/addons/detail/keepassxcbrowser/pdffhmdngciaglkoonimfcmckehcpafo)

Configure KeePassXC-Browser 

Open the KeePassXC application on your desktop and navigate to Tools > Settings. Then click the Browser Integration option on the left-hand side (1). The following screen appears:

![10](https://user-images.githubusercontent.com/113516460/221550712-883fabdb-94b1-4763-a6a5-b33ae1d70221.JPG)

Click the Enable browser integration checkbox (2). Then select the browsers for which you have downloaded the KeePassXC-Browser extension (3) and click OK. Ensure your database is unlocked, then open (or restart) your browser. Click the KeePassXC-Browser extension icon (A) in your browser (see figure below). A pop-up window appears.

![11](https://user-images.githubusercontent.com/113516460/221551756-eb853876-6210-4454-852a-5ae91797de31.JPG)

Click the Connect button (B) in the pop-up window to complete integrating the KeePassXC-Browser extension with your KeePassXC desktop application.

You are now prompted to enter a unique name to identify the connection between this browser and your database. Enter a unique name in the field (e.g., firefox-laptop) and click the Save and allow access button.
![12](https://user-images.githubusercontent.com/113516460/221551934-a647ea6e-99c7-416d-bbd4-50c28e4590a3.JPG)

So, now that everything is set up. Lets see the status of the KeePassXC on the browser. 

1️⃣Open your KeePassXC desktop application and unlock your database.
2️⃣Open your web browser. The KeePassXC-Browser extension icon in your browser window will change based on its connection state. The figure below shows the different states.

![13](https://user-images.githubusercontent.com/113516460/221552319-74405ea8-40a0-41ae-9600-7c9d83f2d43a.JPG)

Encrypt and decrypt a message (you can use any tool you want, gpg is one option)
---------------------------------------------------------------------------------------
A problem that many users face is how to communicate securely and validate the identity of the party they are talking to. To get around this issue, GPG relies on a security concept known as public key encryption. The idea is that you can split the encrypting and decrypting stages of the transmission into two separate pieces. That way, you can freely distribute the encrypting portion, as long as you secure the decrypting portion. This would allow for a one-way message transfer that can be created and encrypted by anyone, but only be decrypted by the designated user. Another benefit of this system is that the sender of a message can “sign” the message with their private key. The public key that the receiver has can be used to verify that the signature is actually being sent by the indicated user.

For this task I will use GPG in order to encrypt and decrypt a message. 

Our first job is to set up the keys. 

        $sudo apt-get update
        $sudo apt-get install gnupg
        
To begin using GPG to encrypt your communications, you need to create a key pair. You can do this by issuing the following command:

![1](https://user-images.githubusercontent.com/113516460/221990116-4cc6ac2d-8348-4e37-990e-b4c2f116ef72.JPG)

At this point, gpg will generate the keys using entropy. Entropy describes the amount of unpredictability and nondeterminism that exists in a system. GPG needs this entropy to generate a secure set of keys.

At this point I encountered some issue and I will try to resolve it and update it to wednesday's course. 

:)


SOURCES :globe_with_meridians:
________________________________________________________________________________________________

    https://www.cnbc.com/2022/12/27/benefits-risks-of-using-a-password-manager-to-protect-online-identity.html
    https://www.lastpass.com/
    https://blog.envisionitsolutions.com/5-benefits-of-using-a-password-manager
    https://campaigns.f-secure.com/id-protection/pm/fi/?gclid=EAIaIQobChMIpKHIj8u1_QIV8AuiAx1JMAEaEAAYASAAEgIDW_D_BwE&gclsrc=aw.ds
    https://keepassxc.org/docs/KeePassXC_GettingStarted.html#_application_layout
    https://www.logmeonce.com/blog/password-management/7-benefits-of-using-password-management-software/
    https://www.digitalocean.com/community/tutorials/how-to-use-gpg-to-encrypt-and-sign-messages
    




