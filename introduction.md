## Introduction to Blockchain technology

## 

In 2008 Satoshi Nakamato wrote a paper entitled “Bitcoin: A Peer-to-Peer Electronic Cash System”. In this paper, Satoshi explains what would later become known as “blockchain technology”. He describes it as:

* A peer-to-peer electronic system for financial transactions without going through a bank
* The use of \(hashing\)cryptography instead of trusting a bank
* The creation of trust through the system without the use of centralized institutions

---

#### **Words to know:**

**Hashing**- generating a value from a string of text using a mathematical algorithm

**peer-to-peer network**-A network** **of computers configured to allow certain files and folders to be shared with everyone

**ledger**-an account book of final entry, in which business transactions are recorded.

**proof of work**- requiring processing time of the computer \(to create the hash from a mathematical function in this case\)

**blocks**-a record of business transactions\(ledger\) where computers have spent time finding the answer to an algorithm\(hash\)

---

To avoid double-spending problem Satoshi Nakamato determined that a network of timestamps could be distributed over the peer-to-peer network \(a type of ledger file\) in the form of a hash-based proof-of-work which would create a record that could not be changed without redoing the proof-of-work. These hashed proof of work records are now known as blocks.

Once the hashing was complete for a block and 51% or more of the computers on the network agreed, the block was added to the one previous block to create a blockchain and distributed to the network. A new block would then be  hashed. If there were any changes made to any block on any computer in the peer-to-peer network, also called nodes, that change to the block would need to be rehashed and the resulting newly hashed block would have a different hash code and therefore it would not be accepted by 51% or more of the nodes and therefore rejected.  In Ethereum blockchain here are 2 things the nodes must agree on before a block can be added. The hash from the previous block\(called the block header\)  and the Merkle root.  Below is a tree that shows how each block in is not only the all transactions that have taken place in the block's time frame but also the hash of the 2 below it. Bitcoin does not use the Merkle tree system.

![](/assets/Merkle Tree.jpg)

In this way, no single node can change the blockchain nor could a group of bad actors. It would require 51% or more of the nodes to agree to a change which is virtually impossible. Hackers are aggressive; however, it has been estimated that the amount of computing power it would take in order to register 51% of the nodes in the bitcoin node system is over 500 of the fastest computers in the world.

What is hashing? It is the transformation of a string of characters into a key or value that represents the original values. Hashing is used all the time in computer systems. Imagine a list of names such as John Drum, Sue Wilson, William Smith, Tom Jones. If each person’s information were stored in a database using their name as the key, a request to retrieve someone’s information would require the computer to search every single letter one by one to confirm whether it matched or not before going onto the next name and repeating the process until it found a match. It could then retrieve the data. However, computers use algorithms and information would be stored something like this: 2344 John Drum, 6388 Sue Wilson, 6901 William Smith, 6395 Tom Jones. In computers, the request would go to each number associated with the person’s name as a key to find a match and the same request process could be completed much faster. An actual hash would be much longer and more complex but the example above provides the basic concept. Hashing is used for both speed and security in computer systems.

Let’s go see an actual hashing algorithm in action. Go to the website listed below:

[http://www.sha1-online.com](http://www.sha1-online.com/)

![](/assets/SHA-1.jpg)

Enter “hello world” and click the “hash” button.

![](/assets/hello world2.jpg)

Notice that the hashed result is a 40-digit hexadecimal number.

Now remember the first few characters and change something in the original “hello world” entry we made. For example, capitalize one letter or add a period at the end. When you have made the change click the hash button again.

![](/assets/Hello world capital.jpg)

Notice that the SHA-1 hexadecimal number changed. Now change the entry back to “hello world” and notice that the number is the same as the first time you entered it.Any change whatsoever to the data in the box will result in a new hash number.

Let's revisit the Merkle root concept. below is a short list of transactions that might have taken place in a typical block's time. Copy and paste them into the SHA1 hash box click "hash" and look at the result.

> John pays Sue .0000012 ETH
>
> Will pays Neal .0000000036 BTC
>
> Mike pays Carol .0000000421 BTC
>
> Robin pays Steve .000000024 ETH
>
> Wilson Electrons agrees to pay VoltsRus $16,000 USD on July 16th for 1200 CPU units to be delivered on July 1

\(the bottom line is an example of a simple smart contract. More on this later\)

The resulting hash is an example of a Merkle root. Try to change or add even 1 thing and click the hash button again and the hash changes. No single bad actor could change the blockchain \(the Merkle root of a single block in this case\) once it's hashed. Even if several bad actors got together it would be impossible because of the 51% consensus required to write each block to the chain. Additionally, any Merkle root in the past could not be changed because all the blockchain's hashes up to the current block would have to be rehashed.

Why would someone want to hash all the transactions? Because the person who finds the answer to the cryptographic algorithm is rewarded a coin or coins. \(Bitcoin currently awards 12.5 coins to a person who discovers the correct hash\)

In Ethereum, each block takes approximately 15 minutes to hash. Ethereum controls the difficulty of the algorythm based on the number of nodes currently hashing the block and the speed at which they are doing it. If you want to see the Block Rate you can go to this website.

[https://etherscan.io/chart/blocktime](https://etherscan.io/chart/blocktime)

![](/assets/block rate.jpg)

Hashes are called one-way encryption. This means that it is impossible for a computer program to reverse engineer the hash to get to the original data. Hashes are constantly evolving as new security concepts arise and new ways of hacking are developed. The SHA-1 stands for “Secure Hash Algorithm 1” and was developed by National Security Administration\(NSA\) in 2005. Since 2010 many organizations have recommended it be replaced by SHA-2 or SHA-3. Ethereum uses SHA-2.

Hopefully you can understand how secure the blockchain technology is. The requirement that a minimum of 51% of the nodes approve a block before it is added to the blockchain, along with the proof-of-work via hashing, make blockchain technology more secure than current banking systems.

