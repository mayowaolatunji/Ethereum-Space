---
description: >-
  Smart contract code execution is accomplished because the EVM functions to
  update the Ethereum state by validating state transitions. This document will
  disclose what constitutes the Ethereum state.
---

# Ethereum state

## Introduction

The EVM acts as a mathematical function that produces a deterministic output given a specific input. Ethereum is therefore described as a state transition function.

**Y(S, T)= S'**

where(S)= old valid state

(T) = a new set of valid transactions,

Y(S, T) = is the Ethereum state transition function

S' = produces a new valid output state.

## The state Transition function

When a transaction is initiated through a smart contract, the EVM is instantiated with the details of the block & transaction. the state transition function establishes the transaction validity, order, and structure.

Below is the constituent of the Ethereum state: The Ethereum top-level world state consists of the mapping of addresses. while the lower level, every Ethereum address represents an account containing an ether balance, a nonce, the account’s storage, and the account’s program code(only if the account is a smart contract account).

The transaction fee is estimated by the price of gas, while the sender's address is determined using the signature. A user sending coins from an address is settled with a reduced account balance along with the increment of the nonce. If there is no sufficient balance, an error or halt will be initiated.
