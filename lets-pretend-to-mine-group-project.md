# Let's pretend to mine Ethereum

What is actually happening when crytocurrency miners are mining? What are they doing? Remember our example earlier? Let's use it to start mining for Cryptocurrency. We'll do it by hand so you can see what's happening. There's no programming or algorithms required for our group mining project.

First copy this list of transactions below. This will be block \#1.

> John pays Sue .0000012 ETH
>
> > Will pays Neal .0000000036 BTC
> >
> > Mike pays Carol .0000000421 BTC
> >
> > Robin pays Steve .000000024 ETH
> >
> > Wilson Electrons agrees to pay VoltsRus $16,000 USD on July 16th for 1200 CPU units to be delivered on July 1

Now let's go back to a different  SHA-1 Hash Generator and hash it.

[https://passwordsgenerator.net/sha1-hash-generator/](https://passwordsgenerator.net/sha1-hash-generator/)

![](/assets/Hash generator3.jpg)

## The result is our Merkle Root for block \#1! --&gt; 6A4611D80B461B9BC90A82F6F18D6B041828E503

---

# First let's dive a little deeper into what exactly a block is...

### Every _Block_ consists of 5 things:

1. Block Header \(see below\)
2. Block Size
3. Magic number \(used to identify the file/data structure\) 
4. Transaction counter
5. Transactions

#### Every  _block header_ consists of 6 things:

1. Version
2. Hash of the previous block
3. Hash of the Merkle Root
4. Time
5. Bits
6. Nonce \(This is the only thing that can be changed during mining\)

### 

---

This graphic should help you understand.![](/assets/blockchain.jpg)

Now let's go back and create our **block header** for our first block and hash it.

> version 1.0
>
> 0000000000
>
> 6A4611D80B461B9BC90A82F6F18D6B041828E503
>
> 9:00:00
>
> 616
>
> 3211

### Our first Block Header hash is below. ![](/assets/Blcok 1 header hash2.jpg)

---

## **This is our header hash from block \#1:**

> 339E3CF37D00CC925B17D47787229EC63FEB39A9

---

### Now we can create block \#2 and mine it

First we need the 5 things to create our block \#2 header \(see above\) 

> 1.0  \(version\)
>
> 339E3CF37D00CC925B17D47787229EC63FEB39A9 \(hash of the previous block header\) 
>
> Hash of the Merkle root for block \#2 we'll need our block \#2 transactions for this\(see below\) 
>
> 09:15:00 \(time\)
>
> 784 \(bits\)
>
> ???? \(Nonce- is a 32 bit binary number meaning only 1's and 0's \)

Let's hash the transactions for block \#2 

\(Note these transactions are continually happening and being distributed via the node network  while the miners work on the answer to the hash\)

> Andre pays Phillip .000000003372 BTC
>
> Wang Fang pays Zhang Wei 1.229000012 ETH
>
> Juan pays Antonio ..00022100002 ETH
>
> Joe's Burgers agrees to pay Buddy's beef $4000 USD on Sept. 30 for 1000 pounds of custom ground beef containing no more than 10% fat to be delivered on Sept. 1
>
> Leon agrees to pay Finn 2.3309733 ETH

Copy and paste the transactions above to SHA1 website to get the hash.

![](/assets/Block2 Merkle.jpg)

### So the Merkle Root for block \#2 is 

> 907568856696392D5781D625333A8270E8E253E0

### 

### Now we have everything necessary to create block \#2 and collect our cryptocurrency coins! 

---

## BUT WAIT!  There's a problem.... and a challenge!

In order to meet the difficulty level, Ethereum is requiring that our hash for our first block begin with a 0 \(zero\)! 

Your **FIRST challenge** is to  copy block \#1 "Block Header" information \(see below\)  and change the nonce \(and ONLY the nonce\) in order to solve the computational problem to create a hash that begins with a zero. 

Your **SECOND challenge** is to see who can find a nonce that creates the MOST leading zeros in the hash. You can use up to 20 digits but only use numbers.

Your **THIRD challenge** is to create 3 or 4 transactions for block \#3 and mine block \#2  hash that starts with a 0 \(zero\)

---

## Difficulty level of cryptocurrency mining

Bitcoin miners at the time of this writing must find a hash with 17 leading zeros. You can go to the link below to see the info on most recent completed blocks. Everything is listed there. 

[https://blockchain.info/blocks](https://blockchain.info/blocks)

Normally the nonce is a 32 bit binary number. By adjusting the required number of zeros based on the number of miners and their combined computing power the cryptocurrency networks can adjust the number of leading zeros to make the chain production time consistent. 

How many possible combinations are there in a 32 bit binary number?  4,294,967,296 Yes, over 4 billion!

