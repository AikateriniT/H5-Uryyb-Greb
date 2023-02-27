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

KeePassXC places controls over the access to this data so other applications cannot read it (unless they have administrative rights). By default, KeePassXC prevents recordings and screenshots of the application window on Windows and macOS. This prevents inadvertent spillage of information during meetings and disallows other applications to capture the window contents.

With these two password managers the encryption used is AES-256 The Advanced Encryption Standard (AES), also known by its original name Rijndael, is a specification for the encryption of electronic data established by the U.S. National Institute of Standards and Technology (NIST) in 2001.

The Advanced Encryption Standard (AES) is defined in each of:

FIPS PUB 197: Advanced Encryption Standard (AES)
ISO/IEC 18033-3: Block ciphers

For additional security steps:

Users can add Twofish or ChaCha20 encryption for an extra layer of security. It is also compatible with Yubikey (a USB multifactor authentication method) for supreme security of the KeePassXC database file. 

Demonstrate the use of a password manager.
-----------------------------------------------------------------------------------------------

I will demonstrate you the use of KeePassXC because this is the one that I am using and I am familiar with. 

The reason I prefer it, is because it has a clean and understandable interface and it is easy to use. It is an application that supports all operating systems (windows, macOS, Linux) and it does not have a mobile app.  
________________________________________________________________________________________________

Let's start from the beginning though, with the first steps of installation and creating a new user. 

    - Step 1: Download KeePassXC application and create a new database.

https://keepassxc.org/download/
________________________________________________________________________________________________
Note!
Before installing KeePassXC, you should always verify that your download matches the signature that is published alongside the release package!

Warning: Please do not download unofficial packages from sources you don't trust!

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

    1. You have to add a title for your entry.
    2. Then the username
    3. Add the password, which can be chosen by you or can be generated by clicking the small square next to the 
    visible/invisible button.
    4. The URL. After you add a URL to an entry you can press the download button to automatically download the 
    website’s icon for this entry.
    5. Add tags if you wish 
    6. An expiration day, which means that the manager will ask you to change your password.
    7. Add notes for this website. 
    
Generate a random password with the password generator by clicking the small square buttton. 

![8](https://user-images.githubusercontent.com/113516460/221538384-43e63190-9034-4f56-8a69-de9c0d96af26.JPG)

From the choices 1,2,3,4 you can pick what kind of characters you want to be included to your password. Some websites do not allow all kinds of special characters for example. Then from number 5 you can choose how many characters long you want your password to be. The green bar under the password shows you how strong your password is. 

Using KeePassXC as an authenticator app by adding TOTP to an entry. 
__________________________________________________________________________________________
The KeePassXC database offers also the option to use it as an authenticator app, by adding a TOTP to an entry. It is exactly the same as Google Authenticator or any other authenticator.

Timed One-Time Passwords is a two-factor authentication method. These codes are typically six digits long and change every 30 seconds. They are derived from a shared secret value and the current time. Once set up, KeePassXC can calculate TOTP codes like any authenticator app, such as Google Authenticator. The codes can be used with copy/paste, browser extension, and Auto-Type.

Note! The computer must be synchronized with the internet time source in order to generate valid TOTP codes. 

Warning! It is wise to create one database for the passwords and another one for the TOTP codes. In this case the benefits of two-factor authentication will not be eliminated. The TOTP database is good to be unlocked only when needed. 

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







