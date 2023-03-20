# Mikasa

Modular Ink-based Kinetic Autonomous Smart Contracts Architecture.

## Overview

The goal of this project is to create a Substrate pallet that allows to execute autonomous smart contracts that are written in Ink!. It can be used to do automatic onchain actions, triggered by the protocol, without requiring any user interaction. For instance, it can be used to implement a ticker function for some onchain games. 

The scope of the hackathon is to implement an onchain fully autonomous Game of life contract that is written in Ink! and deployed on a Substrate node with the contracts pallet enabled.

## Components

- [ ] Autonomous smart contracts pallet
- [ ] Game of life Ink! contract
- [ ] Game of life frontend
- [ ] Documentation
- [ ] Demo video

Optional / Bonus:
- [ ] Price oracle Ink! contract


## Architecture

The main components of the system are:
- `gol`: the Game of life Ink! smart contract
- `gol-app`: the Game of life frontend
- `mikasa-node`: the Substrate node with the autonomous smart contracts pallet enabled

Optional / Bonus:
- `price-oracle`: the Price oracle Ink! smart contract

### Autonomous smart contracts pallet

The autonomous smart contracts pallet should be a Substrate pallet that allows to execute autonomous smart contracts.

The pallet should be able to execute autonomous smart contracts that are written in Ink! and deployed on a Substrate node with the contracts pallet enabled.

### Game of life Ink! contract

The Game of life contract should be an autonomous smart contract that is written in Ink! and deployed on a Substrate node with the contracts pallet enabled.

The contract should be able to execute the game of life algorithm and update the state of the game of life.

### Game of life frontend

The frontend should be a web application that allows to interact with the Game of life contract.

The frontend should be able to display the state of the game of life and allow to interact with the contract.

### Documentation

The documentation should be a markdown file that explains how to deploy the autonomous smart contracts pallet and the Game of life contract on a Substrate node with the contracts pallet enabled.

### Demo video

The demo video should be a video that shows how to deploy the autonomous smart contracts pallet and the Game of life contract on a Substrate node with the contracts pallet enabled and how to interact with the Game of life contract using the frontend.


## Resources
### Substrate & Ink!
- [Ink! documentation](https://use.ink/)
- [substrate node with contracts pallet enabled](https://github.com/paritytech/substrate-contracts-node)

### Massa
- [Autonomous smart contracts documentation](https://docs.massa.net/en/latest/general-doc/autonomous-sc.html#general-asc)
- [Massa: Autonomous smart contracts from dapp developer perspective](https://docs.massa.net/en/latest/general-doc/autonomous-sc.html#general-asc)
- [Massa: Dapp example of an oracle using autonomous smart contracts](https://github.com/massalabs/massa-sc-examples/blob/main/ticker/assembly/contracts/oracle.ts#L25)
- Execution of an autonomous smart contract: [massa-execution-worker execute_async_message function](https://github.com/massalabs/massa/blob/main/massa-execution-worker/src/execution.rs#L695)
- Read asynchronous messages to execute: [massa-execution-worker execute_slot function](https://github.com/massalabs/massa/blob/main/massa-execution-worker/src/execution.rs#L819)

### Game of life frontend
#### Game of life React

- https://github.com/creotip/game-of-life-react
- Demo: https://game-of-life-app.netlify.app/
- Tutorial: https://creotip.io/posts/building-game-of-life-with-react-hooks-chakra-ui

#### Rust Wasm Game of life

- https://github.com/rustwasm/wasm_game_of_life
- https://rustwasm.github.io/docs/book/game-of-life/introduction.html