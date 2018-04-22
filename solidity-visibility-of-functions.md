# Visibility of Functions

###### There are 4 levels of visibility of functions.

* **External- functions that will not be called from your contract but that will still be visible to other contracts**
* **Public- any contract or anyone can access your contract**
* **Internal- can be accessed within the contract and by any contract that is derived from the contract\(any child has access\)**
* **Private- is only accessible within the contract**

Any function that is not set by using one of the key words above defaults to **public**. Note the difference between **Public** and **External** is how the parameters are called. If the function is marked as **public** there is a copy made of the parameters which are stored in **calldata**. If the function is marked as **External** the parameters are read directly from** calldata** without making a copy therefore making the cost of gas much cheaper. You may remember from the section titled "Understanding EVM memory" we discussed that **calldata** is a special place in the EVM memory where parameters are stored. You can't modify parameters that are in **calldata** nor do parameters in **calldata** persist.

Some examples of of fuctions with visibility settings. 

```
pragma solidity ^0.4.21;

contract mycontract {
    function checkData(){
        setData(7);
    }

    function appleCount (uint a) private returns (uint){
        returns a +1;
        }

    function setData(uint a) internal {
        returns data = a;
        }

    function outside() external returns (uint) {
        return 12;
        }

    function totalApples (uint) public returns (uint){
        returns a;
        }
```



