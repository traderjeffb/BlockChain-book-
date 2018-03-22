# Setting up the Solidity Development Environment

The first thing we'll need to do is to download Node.js

What is Node.js?

> _Node_._js _ is a JavaScript runtime built on Chrome's V8 JavaScript engine. _Node_._js  \_uses an event-driven, non-blocking I/O model that makes it lightweight and efficient. \_Node_._js _ package ecosystem, npm, is the largest ecosystem of open source libraries in the world.
>
> source:[https://nodejs.org](https://nodejs.org)

Start by going to this link: [https://nodejs.org/en/download ](https://nodejs.org/en/download/)

Choose the proper download for your computer. Once it gets done downloading double click on the file and a pop-up screen will appear. Click on the 'Run" button. Once you click on "Run" you'll see the install wizard- click  through all the default settings. The installation could take a while. Be patient. ![](/assets/Node.jpg)

Next we need to install Truffle but to do so we need to go the the command window DOS prompt. To get there, Click on the start button in the lower left hand corner of your screen. in the search box to the right of the start button type "cmd" and hit enter. This will bring up a black box. Once you see the black box type in "npm" as shown below:

![](/assets/npm.jpg)

We want to install Truffle. What is Truffle?

> **Truffle**
>
> is a development environment, testing framework and asset pipeline for **Ethereum**, aiming to make life as an **Ethereum**
>
> developer easier. With **Truffle **, you get: Built-in smart contract compilation, linking, deployment and binary management.

Let's go to Truffle's website to see what the command is -follow the link below

[https://www.npmjs.com/package/truffle](https://www.npmjs.com/package/truffle)![](/assets/truffle.jpg)

If you scroll down you'll see the command we need:

\(don't type the "$" sign\) type this command and hit enter.![](/assets/truffle install.jpg)You should see some flashing as truffle installs![](/assets/install truffle.jpg)

What is testrpc?

> [**testrpc **is a Node.js based Ethereum client for testing and development. It uses ethereumjs to simulate full client behavior and make developing Ethereum applications much faster.](https://www.npmjs.com/package/ethereumjs-testrpc)
>
> [source: https://www.npmjs.com/package/ethereumjs-testrpc](https://www.npmjs.com/package/ethereumjs-testrpc)

Let's go to the testrpc website to find the command. Follow the link below

[https://www.npmjs.com/package/ethereumjs-testrpc](https://www.npmjs.com/package/ethereumjs-testrpc)![](/assets/testrpc.jpg)

Scroll down to find the command we need. You should find this:

![](/assets/testrpc install.jpg)Type the line above into the command line and hit enter. 

![](/assets/install testrpc.jpg)

Now let's test to see if everything is on our machine properly. On the command line type "testrpc" and hit enter. You should get a window like the one below. Notice that testrpc gives you 10 account pre-loaded with fake either and 10 corresponding private keys. Below that testrpc tells you the local host is 8545. ![](/assets/testrpc accounts.jpg)

Now let's check to see if Truffle is properly installed. First lets' create a new directory. 

* Type "mkdir proj1" in the command window.
* Now let's enter that directory by typing "cd proj1"
* By entering "dir" and pressing enter we can see that there are 0 File\(s\)
* Now let's initialize Truffle by typing "truffle init" and hit enter
* Finally let's see that Truffle set up some files by typing "dir" and hitting enter

\(follow along with all these instructions below\)![](/assets/testing truffle.jpg)We can see above that Truffle set up the contracts, migrations and test directories and added a couple of files. Everything appears to be working correctly. Now we are ready to write smart contracts using Truffle and testrpc! 

