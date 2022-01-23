# Ethereum Dapp for Tracking Items through Supply Chain
Create a DApp supply chain solution backed by the Ethereum platform. Architect smart contracts that manage specific user permission controls as well as contracts that track and verify a product’s authenticity. The contract has been tested, deployed to Rinkeby public chain, and a web front end has been created for users.

## UML Diagrams

### Activity Diagram
![Activity UML](https://user-images.githubusercontent.com/7294966/150676901-e0b391e8-5aaa-4d39-829c-547759e7f55c.png)


### Sequence Diagram
![Sequence UML](https://user-images.githubusercontent.com/7294966/150676919-a17bfbe5-606e-4b39-a69b-ccc52448a6b5.png)


### State Diagram
![State UML](https://user-images.githubusercontent.com/7294966/150676929-c454c807-1bf1-4b94-86bc-86005ae7d02a.png)


### Classes(Data Model)
![Classes](https://user-images.githubusercontent.com/7294966/150676944-457d2eaa-ea28-4898-ad5c-8e6f34bec6ee.png)


## Libraries Write-up
The "Roles" library specified below was used for managing addresses assigned to a role.
```
library Roles {
  struct Role {
    mapping (address => bool) bearer;
  }
```

## IPFS Write-up
IPFS is not used in this Dapp.

## General Write-up
The build of the Dapp has 5 steps:
- Part 1 - Plan the project with write-ups: Create UML diagrams and write-ups for the libraries, IPFS, and in general.
- Part 2 - Write smart contracts: (i) AccessControl (ii) Base (iii) Core
- Part 3 - Test smart contract code coverage: 10 tests targeting all the 10 functions used during an item's life span along the supply chain.
- Part 4 - Deploy smart contracts on Rinkeby: Deploy the smart contracts with Truffle.
- Part 5 - Build the frontend.

The Rinkeby contract address for this project is: TBD
