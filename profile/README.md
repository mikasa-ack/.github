# Mikasa

【M】odular【I】nk-based【K】inetic【A】utonomous【S】mart contracts【A】rchitecture.

## Overview

This project aims to create an on-chain implementation of the famous Game of Life cellular automaton using Substrate, Ink!, and a custom-built Substrate pallet. Our project demonstrates the power of autonomous smart contracts for on-chain gaming.

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
- gol: The Game of Life Ink! smart contract, which implements the rules and state updates of the cellular automaton.
- gol-app: A user-friendly web frontend for interacting with the Game of Life contract and visualizing its state.
- mikasa-node: A custom Substrate node with the autonomous smart contracts pallet enabled, allowing for the execution of Ink! smart contracts without user interaction.

### Autonomous smart contracts pallet

The Autonomous Smart Contracts Pallet is a custom-built Substrate pallet that enables the execution of autonomous smart contracts written in Ink!. It is designed to interact seamlessly with the Contracts Pallet, which is responsible for the deployment and management of smart contracts on a Substrate node.

Key features of the Autonomous Smart Contracts Pallet include:

Triggering smart contract execution on a predefined schedule, such as every block or at specific block heights.
Supporting multiple autonomous smart contracts with varying schedules and execution conditions.
Ensuring compatibility with the Contracts Pallet and other Substrate runtime modules.

### Game of life Ink! contract

The Game of Life contract is an Ink! smart contract that implements the rules and state updates for the Game of Life cellular automaton. It features:

An on-chain representation of the Game of Life grid with a configurable size.
Functions for initializing the grid, updating the grid state according to the Game of Life rules, and querying the current grid state.
Autonomous execution of state updates, leveraging the Autonomous Smart Contracts Pallet to perform updates without user intervention.

### Game of life frontend

The Game of Life frontend is a web application that provides users with an interactive interface for the Game of Life contract. Its features include:

Displaying the current state of the Game of Life grid with a clean and responsive visualization.
Allowing users to interact with the Game of Life contract, such as initializing the grid, starting/stopping the simulation, or manually updating the grid state.
Connecting to the mikasa-node and automatically updating the grid visualization as new blocks are processed.

### Documentation

The documentation should be a markdown file that explains how to deploy the autonomous smart contracts pallet and the Game of life contract on a Substrate node with the contracts pallet enabled.

### Demo video

The demo video should be a video that shows how to deploy the autonomous smart contracts pallet and the Game of life contract on a Substrate node with the contracts pallet enabled and how to interact with the Game of life contract using the frontend.


## Resources
### Substrate & Ink!
- [Ink! documentation](https://use.ink/)
- [Substrate general documentation](https://docs.substrate.io/)
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
