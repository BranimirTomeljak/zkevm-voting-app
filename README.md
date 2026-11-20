# zkEVM Voting: App

React client for the on-chain voting system built for my MSc thesis, *Non-interactive Zero-Knowledge proofs in blockchain* (FER Zagreb, 2025). It talks to [zkevm-voting-contracts](https://github.com/BranimirTomeljak/zkevm-voting-contracts) on the Polygon zkEVM Cardona testnet through MetaMask.

<!-- Screenshots: add 2–3 here (current election, past elections, admin panel). -->

## Features

- Connects a MetaMask wallet and follows account and network changes
- Shows the current election with its candidates and vote counts, and lets verified users vote once
- Lists the results of past elections
- Admin panel for the contract owner: add candidates, start, end and create elections, and verify or unverify voters
- Self-verification for the demo (see the note in the contracts README)

## Stack

React 19 · TypeScript · Web3.js 4 · Create React App

## Running locally

You need MetaMask connected to the Polygon zkEVM Cardona testnet.

```bash
npm install
npm start   # http://localhost:3000
```

Contract addresses are in `src/util/constants.tsx`, and the ABIs are in `src/contracts/`.
