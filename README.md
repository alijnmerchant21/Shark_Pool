# Shark_Pool
Shark Pool based on DApp. 

The function of the DApp is very simple. We have created a pool, where people can contribute their Ether upto a specific deadline.
Pass the deadline, the deposit of ether completely stops.
The shark of the pool; that is the account making the highest amount of contribution gets all the ether in the pool.

*Skeleton*

1. Withdraw function.
2. Deposit function. (Public Payable Function.)

Truffle by default provides acccess to - 'Web3', 'Mocha' and 'Chai' libraries.

**Artificats.require():
To fetch code abstraction - There is no need to (require) contracts ABI or bytecode.

**contract()
This is similar to describe() in Mocha. The only key difference is it gives you account parameter which can be fetched from web3.

**beforeEach()
This is same in Mocha. It gets called before each it() function. This way you get a new contract for each test.

**contract.now()
Deploys a new instance of the contract. Only the parameters of the constructor need to be mentioned.

**Goals of Backend Service:
Get data from blockchain and store it for easier access.
Perform data analysis and data manipulation.
Designed for data recovery from blockchain.
Event based design; it should work with multiple blockchain input. (RPC, WebSocket, etc.)
Transaction can be rejected or removed, because the uncle block needs to be robust.

**Backend Implementation:
Using Node.js with MongoDB and Express framework.
Parsing of data is done via Web3.library.

**Contract storage:
Accessible within contract.
32 Bytes -> 1 storage unit.
20,000 Gas -> To change value. This value is even less, if the variable is already set and only value is changed.

**Log event:
Triggered from within the contract; permenant and irreversible storage.
Cannot be accessed from within the contract.
Much cheaper - 375 Gas per log, plus 8 gas per byte in the log.

**Geth:
Go Ethereum is a command line interface for running full ethereum on go.

By installing and running Geth, you can take part in Ethereum frontier live network and:
- Mine real ether.
- Transfer fund between addresses.
- Create contract and send transactions.
- Explore Block history.
