# CounterDapp

# Simple Counter DApp Contract

This is a beginner-friendly guide to creating a simple counter decentralized application (DApp) contract using Solidity and deploying it using Remix.

## Prerequisites

- Install [Remix](https://remix.ethereum.org/), an online Solidity IDE.

## Getting Started

Follow these steps to create and deploy your own simple counter DApp contract:

### Step 1: Set Up Your Development Environment

1. Install Remix: Open your browser and go to [Remix](https://remix.ethereum.org/).

### Step 2: Create a New Solidity File

1. Open Remix in your browser.
2. Click on the '+' icon in the file explorer panel to create a new file.
3. Name the file `Counter.sol`.

### Step 3: Write the Counter Smart Contract

Copy and paste the following Solidity code into the `Counter.sol` file:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract SimpleCounter {
    uint256 private count;

    constructor() {
        count = 0;
    }

    function getCount() public view returns (uint256) {
        return count;
    }

    function increment() public {
        count += 1;
    }

    function decrement() public {
        require(count > 0, "Count cannot go below zero");
        count -= 1;
    }
}

 

```
### Step 4: Compile and Deploy the Contract
In Remix, ensure that the Counter.sol file is open.
Click on the "Solidity Compiler" tab in the left sidebar.
Choose the appropriate compiler version (e.g., 0.8.0).
Click the "Compile Counter.sol" button.
### Step 5: Deploy the Contract
Click on the "Deploy & Run Transactions" tab in the left sidebar.
Select the "Injected Web3" environment.
Click the "Deploy" button next to the SimpleCounter contract.
### Step 6: Interact with the Contract
After deploying, you'll see your contract interface.
You can call the getCount() function to see the current count.
Use the "Write" section to call the increment() and decrement() functions to modify the count.
### Congratulations! You've created a simple counter DApp contract and deployed it using Remix 🎉.
 






