# Smart Contracts

Smart contracts are self-executing contracts with the terms of the agreement directly written into code. They run on blockchain platforms like Ethereum.

## Key Concepts
- **Code Execution**: Contracts automatically execute when conditions are met.
- **Immutability**: Once deployed, contracts cannot be altered.
- **Decentralization**: Operate on a distributed network.

## Example Code
### Solidity: Simple Smart Contract
```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract SimpleStorage {
    uint256 public storedData;

    function set(uint256 x) public {
        storedData = x;
    }
}
```

## Learning Resources

- [Smart Contracts - Ethereum](https://ethereum.org/en/developers/docs/smart-contracts/)
- [Building Smart Contracts - YouTube](https://www.youtube.com/watch?v=Z2qv2hmKLYs)

## Next Steps

1. Develop and deploy your own smart contracts.
2. Explore decentralized applications (dApps) built on blockchain.
