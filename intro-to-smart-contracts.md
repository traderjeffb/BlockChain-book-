# Introduction to Smart Contracts

Let's get started with a simple smart contract and get familiar with the Remix IDE. In the top left corner find the "+" symbol. Click this "+" to create a new contract.

![](/assets/Create new file.jpg)

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

![](/assets/pragma solidity.jpg)Now we must name our contract in our code. Note, everything for this contract must be written between these two curly braces. If you enter the first curly brace at the end of the line and hit enter, Remix will add the bottom one for you.

![](/assets/naming contract.jpg)

Next, let's set a define a local variable for type address owner  \(see below\) We'll pass in the address of the owner as the argument of the function. ![](/assets/address owner.jpg)

Now look over on the right hand side. There is a button that says "Start to compile" and a check box beside it for "Auto Compile". Either choice is fine. First check the "Auto Compile" checkbox. Then delete one of the semi-colons you'll see an error message pop up and a red "X" on the number line of the editor. If you hover your mouse over the red "X" it will also give you a pop up error message box. If you want to see these error messages as you code, leave the boxed checked. If you do, you'll find yourself closing error message boxes in the tab section often. On the other hand, there'll the occasionally you'll forget to compile your program after correcting an error and it drive you crazy. \(you have to compile the program each time you make a change.![](/assets/error messages auto compiler.jpg)



