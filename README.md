![nodeCrypto logo](https://www.storix.com/wp-content/uploads/2017/06/encryption-300x260.png)
=============

* * *

*   [What is nodeCrypto?](#what-is-nodecrypto "What is nodeCrypto?")
*   [Install server](#install-server "Install server")
*   [Install and run](#install-and-run "Install and run")
*   [Screenshot](#screenshot "Screenshot")

### What is nodeCrypto? ###  
nodeCrypt is a linux Ransomware written in NodeJs that encrypt predefined files.  
This project was created for educational purposes, you are the sole responsible for the use of nodeCrypto.

### Install server ###  
Upload all file of [server/](https://github.com/atmoner/nodeCrypto/tree/master/server) folder  on your webserver.  
Create a sql database and import [sql/nodeCrypto.sql](https://github.com/atmoner/nodeCrypto/blob/master/sql/nodeCrypto.sql)  
Edit [server/libs/db.php](https://github.com/atmoner/nodeCrypto/blob/master/server/libs/db.php) and add your SQL ID.  

### Install and run ###  
`git clone https://github.com/atmoner/nodeCrypto.git`  
`cd nodeCrypto && npm install`  

You must edit first variable in `index.js`  
Once your configuration is complete, you can start the ransomware.  

`node index.js`

The files at the root of the web server will encrypt and send to the server.  

### Screenshot ### 

![Infection](https://i.imgur.com/eimEruy.png)
![Infection](https://i.imgur.com/ZHUSlLF.png)

### To Do ###  
 - [ ] GUI exe creator
 	 - [ ] Edit basic variable
	 - [ ] Export cross-plateform
 - [x] Client (victim)
	 - [x] Encrypt webserver
	 - [x] Use private key for encryption
	 - [ ] Adapt SSL  
 - [x] Server
	 - [x] Recover data (user + encrypted file)
	 - [ ] Format the database
	 - [ ] Make GUI for webserver
 - [x] Make an executable to decrypt the files (Only on request! Contact me)
