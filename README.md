## Introduction

Solidity, used for writing smart contracts on blockchain platforms like Celo, supports a variety of powerful features. One of these is the `selfdestruct` function, which enables a contract to delete itself and forward its remaining CELO to a specified address. In this challenge, you will construct a contract that can self-destruct under certain conditions.

## Problem Statement

Develop a smart contract that has a self-destruct feature with the following requirements:

1. The contract should allow only the contract creator to self-destruct the contract.
2. The contract should hold a balance.
3. On self-destruction, the contract's balance should be sent to a specific beneficiary address provided by the contract creator.
4. Before self-destruction, the contract should allow the contract creator to change the beneficiary address.

## Hints

- Use the `selfdestruct` function in Solidity to destroy the contract.
- Use `msg.sender` to restrict the self-destruction functionality to the contract creator.
- Store the contract creator's address and the beneficiary address in state variables.
- Use a `modifier` to create a function that only the contract creator can call to change the beneficiary address.

## Evaluation Criteria

- **Correctness**: The contract should compile without errors and fulfill all the requirements.
- **Readability**: The contract should be well-documented, with comments explaining the code.
- **Testability**: You should also provide examples of how to test each function of the contract.

Keep in mind, using `selfdestruct` should be done with caution, as it can make a contract completely unusable and cannot be reversed.

For a comprehensive understanding of Celo smart contracts, Solidity, and the `selfdestruct` function, please refer to the Celo and Solidity tutorials.

## Submission

Please reply with a link to your PR on GitHub, including your self-destructing contract. Also, include any notes or comments you think are necessary to understand your design and choices. Lastly, provide a brief explanation about how each function of the contract should be tested.
