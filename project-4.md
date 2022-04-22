# Documentation of project 4
## Step 1

a. I updated ubuntu
    `sudo apt update`
    ![sudo update](images/image1.PNG)

b. I upgraded ubuntu
   `sudo apt upgrade`
    ![sudo upgrade](images/image2.PNG)

c. I added certificates
    `sudo apt -y install curl dirmngr apt-transport-https lsb-release ca-certificates`

    `curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -`
    
d. I installed NodeJS
   `sudo apt install -y nodejs`
   ![Install nodeJS](images/image3.PNG)

## Step 2
a. I added the key-server
     `sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 0C49F3730359A14518585931BC711F9BA15703C6`
    ![Key server](images/image4.PNG)

b.    `echo "deb [ arch=amd64 ] https://repo.mongodb.org/apt/ubuntu trusty/mongodb-org/3.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.4.list`
       ![Echo](images/image5.PNG)

c.  I installed mongoDB
     `sudo apt install -y mongodb`
     ![IInstall mongoDB](images/image6.PNG)

d.  I started the server and I checked the status
       `sudo service mongodb start`
       `sudo systemctl status mongodb`
       ![Check status](images/image7.PNG)

e.  I installed NPM
        `sudo apt install -y npm`
        ![Install npm](images/image8.PNG)

f.   I installed body-parser
        `sudo npm install body-parser`
        ![Install body-parser](images/image9.PNG)

g.   I created a folder named 'Books'
         `mkdir Books && cd Books`
         ![Mkdir Books](images/image10.PNG)

h.   I initialized the NPM
          `npm init`
           ![npm init](images/image11.PNG)

g.   I added a file named 'server.js' to the Books directory, then I copied and pasted the appropriate code in it.
          `vi server.js`
           ![Server.js](images/image12.PNG)

## Step 3
a.   Install Xpress mongoose
         `sudo npm install express mongoose`
          ![Install express mongoose](images/image13.PNG)

b.   I created a folder named "apps"
       `mkdir apps && cd apps`
       ![apps](images/image14.PNG)

c.   I created a file named "routes.js", then I copied and pasted the appropriate code in it.
       `vi routes.js`
        ![routes.js](images/image16.PNG)

d.  I created a folder named 'models' in the apps directory
     `mkdir models && cd models`
     ![models](images/image17.PNG)

e.  I created a file named 'book.js', then I copied and pasted the appropriate code in it.
     `vi book.js`
      ![book.js](images/image18.PNG)

## Step 4
a.  I changed the directory back to 'Books', then I created a folder named "public"
      `cd ../..` `mkdir public && cd public`
      ![Public](images/image19.PNG)

b.  I added a file named "script.js" then I copied and pasted the appropriate code in it
    `vi script.js`
    ![script.js](images/image20.PNG)

c.  I created a file in the public folder and named it "index.html". Then I copied and pasted the appropriate code in it.
     `vi index.html`
     ![index.html](images/image21.PNG)

d.  I changed the directory back to 'Books'
     `cd ..`
      ![Books](images/image22.PNG)

e.  I started the node server
      `node server.js`
      ![Start server](images/image23.PNG)

f.   I launched a separate SSH console to test what the 'curl' command returns locally
      `curl -s http://localhost:3300`
      ![Curl command](images/image24.PNG)

g.  I launched my public address on my preferred web browser
      `http://184.73.9.165:3300/`
      ![web browser](images/browser.PNG)






        










