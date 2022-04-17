## [![](iconsymbols/home.svg)](index.html)

# Geometron Magic

## A Self-Replicating Set

### Elements

 - [self replicating github repository](https://github.com/lafeLabs/geometronmagic)
 - [global link to replicator code](https://raw.githubusercontent.com/LafeLabs/geometronmagic/main/php/replicator.txt)
 - [solar power station with battery](scrolls/solar)
 - [trash robot open fashion brand: rainbow and googly eyes](scrolls/trashrobotbrand)
 - [Action Geometry: skeletron, s hooks, trash ties, artbox, shape sets, rulers, tiles](http://trashrobot.org/bookofgeometronfirst/user.php?scroll=scrolls/actiongeometry.md)
 - [symbol factory, system of self-replicating vector graphics in the web browser](symbol.html)
 - [icon magic, the system for creating icons which can be replicated in clay, plastic, metal, paper, cardboard, bitmap, vector graphics, laser cut shapes, robot control, building icon printer robots](scrolls/newcoin)
 - free books: the [first book of geometron](https://www.trashrobot.org/bookofgeometronfirst/), [geometron magic](https://www.trashrobot.org/geometronmagic/), [trash magic](scrolls/trashmagic), [trash magic action coloring book](https://www.trashrobot.org/tmacb/) and all of the ideas contained in those books
 - [pi crust media distribution platform](scrolls/picrust)
 - [arduino uno shield for education, motor control, science, neopixels](https://github.com/lafelabs/trashrobot5)
 - [geometron printer with micro positioning for z, two DVD drives, laser optical print and electrode electrochemical print, running geometron](scrolls/microposition)
 - [the roctal system of encoding information in geometry of a surface](scrolls/roctal)


### Links

 - [editor.php](editor.php)
 - [http://localhost/](http://localhost/)
 - [the Geometron Magic github repository](https://github.com/lafeLabs/geometronmagic)
 - [dnagenerator.php](dnagenerator.php)
 - [copy scrolls/home to README.md](copy.php?from=scrolls/home&to=README.md)
 - [scroll set replicator](scrollset.html)
 - [map set replicator](mapset.html)
 - [replicator.php](replicator.php)
 
### Install on Pi

Raspberry Pi is now impossible to buy.  Find them donated from someone. Most people who have them don't use them or used them once and stopped due to lack of interest/time/need. Ask around!  Someone will be able to donate a Pi, keyboard, mouse, screen, power supply and whatever other random things you need to get set up.

Get a SD card with 8 GB or more storage and a SD card USB reader

Download and install, then use the Raspberry Pi Imager:

[https://www.raspberrypi.org/software/](https://www.raspberrypi.org/software/)

Turn on the pi click through all the things, put it on the wifi network.

## Install Apache and PHP so that geometron can run

Open a command prompt(black link on menu bar) and type:

```
sudo apt update
sudo apt install apache2 -y
sudo apt install php libapache2-mod-php -y
```

## Install geometron coin with this document for self-documentation and replication

```
cd /var/www/html
sudo rm index.html
sudo curl -o replicator.php https://raw.githubusercontent.com/LafeLabs/geometronmagic/main/php/replicator.txt
cd ..
sudo chmod -R 0777 *
cd html
php replicator.php
sudo chmod -R 0777 *
```

Check the IP address by hovering over the wifi icon, put that into the browser on another machine on the same local wifi network to see and edit the server.  Or open a browser on the pi and point it to [http://localhost](http://localhost)

## Set up to have names for other servers

edit hosts file to have the IP address of the other servers and then the name you want to use, copying the format in the existing file.

```
sudo nano /etc/hosts
```
edit, and use control-x and say "yes" to save changes.

## connect pi to outside internet over router

Look up "set up port forwarding raspberry pi" and follow instructions to log onto your router and forward port 80 to the raspberry pi.  Use [whatismyipaddress.com](https://whatismyipaddress.com/) to get your global IP address.  Now your home Raspberry pi server will be visible on that IP address.  Take that address and make it a link on the remote raspberry pi terminal as well as a QR code on both.   

edit the /etc/hosts file on the remote pi terminal so that home/ and remote/ point to home pi server either on the local network or on the public network.  So "home" will point to the local IP address on the wifi and "remote" will point to the global IP address of the home raspberry pi server(which everyone can see).  


[link to pi my life up](https://pimylifeup.com/raspberry-pi-port-forwarding/)

[link to setting up basic website with pi with external connection](http://unixetc.co.uk/2013/09/21/create-a-basic-website-on-a-raspberry-pi/)


### Install on Windows or Mac

First, install XAMPP, a free open source web server for all platforms.  [Download from www.apachefriends.org](https://www.apachefriends.org/index.html).  Click on windows to download, and click through to install everything.

![](https://i.imgur.com/G90zeyE.png)

After you download and install it, run it and start Apache.  You should see a control panel like this:

![](https://i.imgur.com/wgpIqfH.png)

Click on "Explorer" to get access to where the files are.  From the main directory called xamp, you want the sub-directory "htdocs".  Open this, delete the index.php file, and create a new file called replicator.php which you copy and paste the replicator at [php/replicator.txt](php/replicator.txt) into, and save.  

![](https://i.imgur.com/EpHYYOd.png)

Point a web browser on the same computer to [http://localhost/](http://localhost), then click on replicator.php.  This should replicate the whole system into the directory.  When this is done, click the link to go to the main page.  

Now you can go [make a new coin](scrolls/newcoin) using your server.

### Install on Android


To run a Geometron Server on an Android, we will install the commercial software ksweb pro.

![](https://i.imgur.com/Q8Q7gaR.jpg)


[link to play store to install ksweb](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwiLrtjPw6fxAhUQu54KHWkyAjIQFjAAegQIBRAD&url=https%3A%2F%2Fplay.google.com%2Fstore%2Fapps%2Fdetails%3Fid%3Dru.kslabs.ksweb%26hl%3Den_US%26gl%3DUS&usg=AOvVaw2ChVP4ojXIuGxVe-JjtEV3)

[https://www.kslabs.ru/](https://www.kslabs.ru/)

Install KSWEB on the Android, and turn it on.  Get the paid version. It is worth it, there are lots of broken web servers out there or ones with crappy features and tons of ads.  This is critical infrastructure for Geometron and it's worth supporting the developer of this useful tool.  Be sure PHP is also turned on.  

This is what it looks like when it is on:

![](https://i.imgur.com/EKjyekx.png)

Use the Editor built into the system to create a new file called replicator.php in the directory htdocs on the sd card as shown above, and to copy/paste into that the file in [php/replicator.txt](php/replicator.txt).  Save that, and delete index.php. Point a browser to the address [http://localhost:8080](http://localhost:8080).  Click on replicator.php and wait for the system to copy.  Sometimes it might time out, try it again.  When the system has replicated, make sure your phone is on a local wifi network, and turn the server off and on again, and you will get an IP address for the phone which is shown in the app.  The link for any other machine on the network other than the phone is the IP address followed by colon and then "8080".  E.g. http://192.168.0.19:8080/.  Share this link via email, text message, and links on other servers so that anyone on your network can see your server and edit it.  

### Replicate the Github using localhost

 - install PHP on your machine
 - create a new github repository on a CC0 PUBLIC DOMAIN license and clone it on your machine
 - copy the file [php/replicator.txt](php/replicator.txt) into a file called replicator.php in the new repo directory
 - run `php replicator.php` on your machine, wait for all the code to copy
 - push all that code up to your github repo
 - in the same directory, type `sudo php -S localhost:80`
 - go to [http://localhost](http://localhost) and you should get back to this screen, edit all elements of the system
 - use [editor.php](editor.php) to edit the file php/replicator.txt so that the two urls are the global url for *your* repo for both dna and replicator
 - after you've edited the code, click [text2php.php](text2php.php) to convert that to php
 - push your code to your github repo
 - use the new replicator code on your github repo to replicate out that instance to all other servers(linux, windows, mac, android) and forks


