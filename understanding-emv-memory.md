# Understanding EMV Memory

It's important that you understand EVM memory. There are 3 levels of memory in the EMV environment 

### STORAGE

### MEMORY

### STACK

**Storage** is used for anything you want to persist. An example is something like a balance. This memory is stored in the EMV environment. 

**Memory **is used to store anything you wish to use within the contract run time. An example might be the results of a computation that you will need to use later in the contract but not after the contract completes running. This memory will only be stored as long as the contract is running. 

**Stack **is the memory  used to run your program in the EMV environment. Think of this as RAM or cache memory of your computer. 



