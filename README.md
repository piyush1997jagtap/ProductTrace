# ProductTrace - Final Project


## Team Members:-
- Sagar Verma - 885163998 - sv2000.sagarverma@csu.fullerton.edu
- Piyush Jagtap - 885147447 - piyush1997jagtap@csu.fullerton.edu
- Pavan Kumar Pasumarthy - 885153056 - ppasumarthy@csu.fullerton.edu
- Akanksh Jagadish - 885199208 - akanksh5@csu.fullerton.edu


## Project Overview:-
Our project will develop a application for counterfeit product identification using blockchain
technology. Each product will be assigned a unique identifier and QR code at the manufacturing
stage, which will be stored and tracked on the blockchain.


## Packages Required:-
- Truffle v5.6.7 (core: 5.6.7)
- Ganache v7.5.0
- Solidity v0.5.16 (solc-js)
- Node v16.20.0
- Web3.js v1.7.4
- npm 7.5.1
- Metamask browser extension

## Features Supported
- Landing page where the user can head to the Manufacturer, Seller Or Consumer.
- As a Manufacturer we can 
    1. Add a Product
    2. Add a Seller
    3. Sell a Product from Manufacturer to Seller
    4. Get the list of sellers using a Manufacturer.
- As a Seller we can 
    1. Sell the Product to a Consumer.
    2. List the Products for sale.
- As a Consumer we can
    1. Check the Consumer Purchase History
    2. Product Verification
- Generate a QR code for a unique Product so that it can be used as a mode of validation. 
    
## Setup process 

1. Clone the project
2. Go to the root folder, and run following command to install required node modules:-
```
npm i
```
3. Compile contract source files. (Compilation and deployment can be done using truffle migrate):-
```
truffle compile
```
4. Open Ganache, (to setup local blockchain)
    - create new workspace
    - add truffle-config.js  in truffle project 
    - change port to 7545 in server settings (same as port in truffle-config.js)
5. In chrome, open metamask 
   - add new test network using  
        - NETWORK ID (i.e. 5777 ,from Ganache Server settings) 
        - RPC SERVER (i.e HTTP://127.0.0.1:7545 ,from Ganache Server settings)
        - CHAIN CODE (i.e. 1337)
   - import account using private key of any account from local blockchain available in Ganache which you just created.
6. Then run the following commands:-
- Run migrations to deploy contracts.
```
truffle migrate
```

- Run the below command to serve the application.
```
npm run dev 
``` 
7. Login to metamask ,and connect the added account to local blockchain manually (i.e.localhost:3000)
