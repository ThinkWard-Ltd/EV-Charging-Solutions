# EV Charging Solution
----------------------

Smart Energy charging is a blockchain-based IoT-platform consists of two parts: JavaScript app and eosio blockchain.

- avaScript Stack:  ReactJS, Redux, NodeJS, Webpack
- Blockchain Stack: EOSIO , IPFS, NODEOS, C++, ABI, Scatter

Users interact with the UI in client and sign the transaction in frontend. The signed transaction is sent to the blockchain directly. After the transaction is accepted in blockchain, the note is added into the multi index table in blockchain.


## JavaScript Stack:  


ReactJS
----------
ReactJS is a declarative, efficient, and flexible JavaScript library for building reusable UI components. It is an open-source, component-based front end library which is responsible only for the view layer of the application. A ReactJS application is made up of multiple components, each component responsible for outputting a small, reusable piece of HTML code. The components are the heart of all React applications. These Components can be nested with other components to allow complex applications to be built of simple building blocks. ReactJS uses virtual DOM based mechanism to fill data in HTML DOM.

Redux
---------
Redux solves this problem by managing application’s state with a single global object called Store. Redux fundamental principles help in maintaining consistency throughout your application, which makes debugging and testing easier, Webpack is a static module bundler for modern JavaScript applications. When webpack processes your application, it internally builds a dependency graph which maps every module your project needs and generates one or more bundles.

Node.js
----------
Node.js is a server-side platform built on Google Chrome's JavaScript Engine (V8 Engine). Node.js is a platform built on Chrome's JavaScript runtime for easily building fast and scalable network applications. Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient, perfect for data-intensive real-time applications that run across distributed devices. Node.js also provides a rich library of various JavaScript modules which simplifies the development of web applications.

Blockchain Stack
-----------------

### What is Blockchain?

Blockchain is a decentralized, distributed store of transaction data. Periodically a new block of transactions is created and connected to the previous block. It is distributed because the blockchain stores transactions across many computers. It is decentralized because the blockchain infrastructure is not owned by one company. Blockchain provides trust; cryptography and consensus ensures that transactions are immutable. Blockchain provides resilience and transparency; decentralization and distribution mean many copies of the blockchain are available for all to see.


### What is a Smart Contract?

An EOSIO Smart Contract is software registered on the blockchain and executed on EOSIO nodes. Smart Contracts implement the semantics of a "contract" and action requests are automatically stored on the blockchain. The Smart Contract defines the interface (actions, parameters, data structures) and the code that implements the interface. The code is compiled for WebAssembly, that nodes can execute.

#

EOSIO
-----------------
The EOSIO software introduces a new blockchain architecture designed to enable vertical and horizontal scaling of decentralized applications. It differs from other blockchains by using features such as DPos as the consensus algorithm and staking for resource allocation. The software provides accounts, authentication, databases, asynchronous communication, and the scheduling of applications across multiple CPU cores and/or clusters. The resulting technology is a blockchain architecture that has the potential to scale to millions of transactions per second, eliminates user fees, and allows for quick and easy deployment of decentralized applications.



### Features of EOSIO:

- High Throughput and Scalability
- Faster Confirmations and Lower Latency
- Feeless and Cost Predictable Blockchain
- Comprehensive Permission Schema
- Upgradability
- Less energy consumption
- Programmable Economics and Governance

#

Building an EOSIO Smart Contract
----------------------------------
Smart contract source code can be written in any language that the WASM (WebAssembly) compiler supports, EOSIO currently supports the C languages (C/C++).


### Transactions and Actions:

A contract and an account communicate in the form of actions. Actions can be sent individually, or batched together if they are intended to be executed atomically. The difference between an action and a transaction is that an action represents a single operation, whereas a transaction is a collection of one or more actions.

### Smart Contract/CDT:

EOSIO.CDT is a toolchain for WebAssembly (WASM) and set of tools to facilitate contract writing for the EOSIO platform. In addition to being a general purpose WebAssembly toolchain, EOSIO specific optimizations are available to support building EOSIO smart contracts.

### Nodeos:

Nodeos is the core EOSIO node daemon. Plugins can be used to configure nodeos to execute with various features. Nodeos handles all peer-to-peer networking, contract code scheduling, and the blockchain data persistence layer.

### Cleos/Keosd:

Keosd is a key manager for EOSIO accounts that comes with EOSIO. Cleos is a command-line tool which let developers interact nodeos as well as deploy, test EOSIO smart contracts.
 
#

EOSJS
-------
A Javascript API SDK for integration with EOSIO-based blockchains using the EOSIO RPC API.


#### Scatter:

Scatter wallet for digital currencies and assets. It’s a multi-blockchain signature, identity, and reputation provider for Windows, Mac, Linux, Android, and iOS.

#

Smart Contract Integration:
----------------------------
EOS API service is created for integrating frontend component with our smart contract We'll also be setting up Redux, which will keep a store of information for us so that we don't need to keep asking the blockchain every time we need the logged in user's name and other information. Redux will use what we call reducers to handle actions that modify the Redux store of state information.

#




