# POO Finance ERC20 Token Swap Smart Contract

This repository contains the code for an Ethereum-based ERC20 token swap smart contract. This contract allows users to deposit ETH and receive $POO tokens in exchange.

## Key Features

- Min Cap:  Users can deposit a minimum of 0.001 ETH
- Max Cap:  Users can deposit a maximum cap of 2 ETH
- Swap Rate:  1 ETH = 11,5200,000,000 $POO
- The contract will close once all 1,600,000,000,000 deposited $POO tokens are exchanged for 138.888 ETH and reject any deposits beyond that with refunds sent back to the sender’s wallet addresses
- The contract is deployed and controlled by the master contract address
- The contract includes a reserve pool that accepts token deposits from any address for any token
- The master contract admin address can withdraw any tokens (both ETH and $POO) deposited into the reserve at any time
- The contract can be updated and redeployed at any time

## Getting Started

To get started with this project, follow these steps:

1. Clone the repository
```bash
git clone https://github.com/yourusername/erc20-token-swap.git


2. Install dependencies
npm install


3. Compile the smart contract
npx hardhat compile


4. Deploy the smart contract
npx hardhat run scripts/deploy.js --network <network>


Testing
To run the test suite, execute the following command:

npx hardhat test
