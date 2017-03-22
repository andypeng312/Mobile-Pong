# README
## Description of Project
This is an app that allows a player to use any accelerometer-enabled device as
a controller to play a game of pong. There are two hard-coded,
password-authenticated users, "bob" and "andy", to use.

The players each log on as one of the users on the "controller.html" page using
their "controller" devices. Using a third device they go to the
"gamescreen.html" page, where they can watch the game of pong that they are
playing. The players move their paddles by tilting their "controller".

![](/Images/mobile-pong.png)

This project uses Node.js and Express.js to run the server on the back end. The
users are authenticated using the Passport.js framework and the controller and
gamescreen pages communicate with the server using websockets through the
Socket.io framework.

The app has been tested between a number of desktop browsers (Firefox, Safari, 
Chrome, IE) and mobile devices (Android, iOS). Debugging was performed using 
weinre, a remote web inspector for debugging web pages on a mobile device.

## Contents
* **`Images`**- contains an image diagramming the concept of the app and
photoshop files used to create it
* **`NodeServer`**- contains all the files for the project, to run:
1. Start terminal in `Bananagrams` directory
2. Start node server by running the command "node server.js"
3. Go to the URL http://127.0.0.1:3000
4. If this is to be used with multiple players on different computers,
replace all instances of "localhost" in the instructions and the code with the
public ip address of the computer hosting the node server
---
**Technologies Used:** Node.js, Passport.js, Express.js, Socket.io, websockets,
HTML5 accelerometer data, weinre (WEb INspector REmote)  
**Estimated Lines of Code:** 800