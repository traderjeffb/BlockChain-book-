# Introduction to Smart Contracts

Let's get started with a simple smart contract and get familiar with the Remix IDE. In the top left corner find the "+" symbol. Click this "+" to create a new contract.

![](/assets/Create new file2.jpg)

---

#### Words to know:

PascalCase- the beginning of every word is capitalized.

camelCase - the first word is not capitalized but every subsiquent word is capitalized.

\(examples:     PascalCase- MyFirstContract.sol          camelCase- myFirstContract.sol\)

---

Remix asks you what you want to name this file. Let's call it "MyFirstContract" Notice the file extension name is .sol - this identifies the file as a Solidity contract. Leave the .sol file extension "MyFirstContract.sol". We'll use PascalCasing when naming this file. Once you rename this file click "OK".![](/assets/name new file.jpg)![](/assets/MyFirstContract.jpg)

You will see your new "MyFirstContract.sol" file listed on the left in the file explorer as well as see the name on the tab. In some projects you may have more than one file open at a time. \(see below\) ![](/assets/MyFirstContractTab.jpg)Now go over to the tab section\( on the right side\)  of Remix and click on settings. Look at the Solidity version. Our current version is "0.4.21" yours may be different. Updates occur frequently. Make note of the version you have and let's begin our program.

![](/assets/Solidity Version.jpg)

Every Solidity program begins by telling the computer which Solidity compiler to use when processing our code. The "Pragma" directive works on Solidity 4.0 and above. Every solidity contract you write will begin with this line of code.

Write the first line using your current version \(if different than the one in the picture below\).  A couple of notes. there's a caret in front of the version of Solidity. The caret is found above the 6. Also, the font is small you can use the plus or minus signs to adjust it to your desired size. I will increase the size now for easier reading.

![](/assets/pragma solidity2.jpg)

Now we must name our contract in our code. Note, everything for this contract must be written between these two curly braces. If you enter the first curly brace at the end of the line and hit enter, Remix will add the bottom one for you.

![](/assets/naming contract2.jpg)

Next, let's set a define a local variable for type address owner  \(see below\) We'll pass in the address of the owner as the argument of the function. ![](/assets/address owner2.jpg)

Look over on the right hand side. There is a button that says "Start to compile" and a check box beside it for "Auto Compile". Either choice is fine. First, check the "Auto Compile" checkbox. Then delete one of the semi-colons you'll see an error message pop up and a red "X" on the number line of the editor. If you hover your mouse over the red "X" it will also give you a pop up error message box. If you want to see these error messages as you code, leave the box checked. If you do, you'll find yourself closing error message boxes in the tab section often. On the other hand, you can compile each time you make a change but there'll the occasionally you'll forget to compile your program after correcting an error and it will drive you crazy. The choice is yours. Read the error message just so you can get experience with what they say. Notice the red "X" doesn't appear on the line where the actual semi-colon is missing. There are things to keep in mind when trying to debug a program.  ![](/assets/error messages auto compiler2.jpg)

Put the semi-colon back into the  program and notice the error message disappears. The name of our contract is on the right now and there's a green bock with the name also that lets us know everything is good. ![](/assets/everything is ok.jpg)

Next, we'll want to set the what environment  we want to run in. On the right hand side, in the tabs section, click the "Run" tab. Click the drop down and chose Java VM. If you were running Mist or MetaMask  you would choose Injected Web3 and if you were running testrpc you could chose "web3 provider". More regarding these last 2 choices later in the course. See below:

\(Again, for now chose JavaScript VM\)

![](/assets/setting run enviorment.jpg)

Below the Environment setting is the "Account" drop down and the "Gas limit". Remix gives you 5 pretend accounts with 100 Ether in each account for you to practice smart contracts. Just leave the it set on the account that it is currently on. The Gas limit default is good for this type of contract. Ethereum will only use up to the amount of Gas set in the Gas limit and no more. In some instances this may result in a loss of gas without your contract being executed.  For more information on Gas read the section titled "Ether, Wei and gas". The "Value" field is used if sending some ether with this contract. We aren't sending any ether so we'll leave it set to 0.  Note below that there's the name of our contract. If we were working on more than one contract we could use the drop down list to access the different contracts. Below that we you can see we are ready to create our first contract!![](/assets/account and Gas limit.jpg)



Let's do something for fun really quick. Let's add another contract. Below "MyFirstContract" let's write a second contract. and call it "MySecondContract". \(see below\)

![](/assets/MySecondContract.jpg)

Now look at the drop down on the right hand side. You can see that both contracts are listed. We can set the drop down to any contract on the list that we wish to interact with. Leave the setting on "MyFirstContract" and delete the lines that were just added for "MySecondContract"

![](/assets/MySecondContract drop down.jpg)

Now click the "Create" button \(see below\)

![](/assets/click create.jpg)



When we clicked create we created an instance of our contract. It pops up. \(see below\)

![](/assets/instance of contract.jpg)





intro....

