
# eris-iot: marmot-proof internet of things engine proposal

## Motivations
Blockchain is a perfect platform for large scale internet of things (IoT) applications.
We have seen tons of thousands IoT devices in recent years, but none of them have 
the ability to solicit their services and process payments. Until recently, IBM 
came up with the proof of concept blockchain-powered IoT network [ADEPT][1], which shows very
exciting and promising applications of blockchain platforms in the realm of machines.
However, the current blockchain infrastructure is so resource-overwhelming for 
the machines and 'blockchain+iot" is so untouched area. To clarify and eliminate 
the gaps, this projects will do:

- Explore the capabilities of IoT devices to run eris blockchain platform.
- Transform the internet of things to blockchain of things with the use of eris-iot.
- Provide better machine experience for blockchain.


## Introduce eris-iot
The eris smart contract application platform provides a really pleasant way to 
integrate blockchain to your project. The code base is modularized and easy to 
use. Following the modularized structure of the code base, the eris-iot complement 
the eris platform for IoT support. The eris-iot should support the IoT devices in 
the following processes:
- Register resource (meta data such as name, type, link, etc.) on blockchain.
- Lookup resource from blockchain. For example, to find the links of nodes that have 
  humidity sensor in the New York area.
- Update resource record on blockchain (in the compliance with the permission model).
- Remove a resource (in compliance with the permission model).
- Mange the permissions for resource directory operations.
- Support payment management for access resources.


## Expected deliveries of this project
To the developer, the best output from the project would be:
- A working API set including all the resource management and permission management 
   features discussed above  of in javascript or other languages. 

To the end user or service providers, the best output from the project would be:
- Configure file interface (XML, or other mark up format file) to add their devices to the 
  blockchain.
- Browser client program to add new node to blockchain using the eris-iot API.

And if possible, we can propose a blockchain-iot standard to IETF or other standard organisation. 

## What I have finished

I have been playing with eris packages for almost a month and have successfully 
ported eris chain management tools to BeagleBone Black and Raspberry Pi 3 evaluation 
boards. And I have tested the following features:
0. Key creation, export and covert.
0. Chain make, new, stop...
0. Setup eris environment on Raspberry Pi using docker machine.

For the smart contract, I wrote a simple device registration and retrieval contract 
and deployed the contract on blockchain running across four nodes (BeagleBone and 
Raspberry PI). And I also wrote javascript application with the following functions:
- Register devices to blockchain
- Unregister devices to blockchain
- Retrieve all devices information from blockchain

## Words from the likely marmot

From a Linux background, I love the modularized architecture of eris stacks and 
the way you (marmot) put all the things together. Both blockchain and IoT are 
revolutions and putting them together has unimaginable power. Joining the marmot 
team, I want to use my IoT experience to power up the marmot in the machine world.
And what I want to get from the marmot are:
+ Learn from smart contract expert.
+ Deep understanding of blockchain system.
+ Experience on industry level blockchain applications.


[1]: http://www.coindesk.com/ibm-reveals-proof-concept-blockchain-powered-internet-things/

