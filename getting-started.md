# Getting Started with CELO Development

This guide will help you get started building on the CELO blockchain.

## What is CELO?

CELO is a mobile-first blockchain platform that makes financial tools accessible to anyone with a mobile phone. It's designed to enable a new universe of financial solutions accessible for mobile users, creating a global financial ecosystem where an end-user can onboard into the CELO ecosystem with just a mobile number.

## Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Basic knowledge of JavaScript/TypeScript
- Understanding of blockchain concepts

## Setting Up Your Development Environment

### 1. Install the CELO CLI

```bash
npm install -g @celo/celocli
```

### 2. Create a new CELO account

```bash
celocli account:new
```

### 3. Connect to CELO testnet (Alfajores)

```bash
celocli config:set --node https://alfajores-forno.celo-testnet.org
```

## Your First CELO Smart Contract

Here's a simple example of a CELO smart contract:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract HelloCELO {
    string public message;
    
    constructor() {
        message = "Hello, CELO World!";
    }
    
    function setMessage(string memory _message) public {
        message = _message;
    }
}
```

## Resources

- [CELO Documentation](https://docs.celo.org)
- [CELO GitHub](https://github.com/celo-org)
- [CELO Discord](https://discord.gg/6yWMkgM)
- [CELO Forum](https://forum.celo.org)

## Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for more details.

## License

MIT License          
