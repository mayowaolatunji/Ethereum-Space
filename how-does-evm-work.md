---
description: >-
  The EVM provides a secure, isolated environment in which to execute untrusted
  code and ensures that the execution of contracts is deterministic and fair.
---

# How Does EVM work?

<figure><img src="https://s3.cointelegraph.com/storage/uploads/view/df7e2dd42b15756c4d2354487bb55468.png" alt=""><figcaption></figcaption></figure>

## Smart Contracts, Nodes, and P2P

Smart contracts are self-executing contracts that define the rules and regulations of an agreement between two parties. The code and data of smart contracts are stored on the Ethereum blockchain, which is maintained by a decentralized network of nodes.&#x20;

These nodes run the Ethereum software and participate in the P2P network, ensuring the consistency of the blockchain. When a smart contract is deployed, the code is executed on each node in the network, ensuring that the same result is obtained regardless of the node that executes it. This ensures the trustworthiness of the smart contract, as the code cannot be altered once it is deployed on the Ethereum network.

## Opcodes, bytecodes & EVM implementation

The code of the smart contracts are written in high-level programming languages such as Solidity, Vyper, or LLL, but it needs to be compiled into bytecode, which is the machine-readable code, before the EVM can execute it. The bytecode is then executed by the EVM, which operates with a set of predefined operations called opcodes.&#x20;

These opcodes are executed one by one, and the state of the Ethereum network is updated with every opcode execution. The EVM implements a stack-based architecture, where the opcodes are executed in the order they are written, and the results are stored on a stack.&#x20;

The EVM also implements a virtual memory space where data can be stored and retrieved, allowing for the execution of more complex computations. The execution of the opcodes is deterministic, meaning that given the same input, the output will always be the same. This ensures the consistency of the Ethereum network, as every node in the network will produce the same result for a given smart contract.

## Gas

The execution of the opcodes on the EVM requires computational resources, which are paid for in Ether, the native cryptocurrency of the Ethereum network. To prevent the execution of an infinite loop or the execution of computationally expensive code, the EVM implements a cost mechanism called gas.&#x20;

Gas is a unit of measurement of the computational resources required to execute an opcode. The cost of executing a smart contract is determined by the amount of gas required for its execution. The sender of the transaction that deploys the smart contract must include sufficient gas with the transaction to cover the cost of its execution. If the gas runs out during the execution, the EVM stops the execution and reverts the state of the network to its previous state.

\
