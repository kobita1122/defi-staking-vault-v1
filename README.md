# DeFi Staking Vault

A professional, secure, and gas-optimized staking smart contract for Web3 ecosystems. This repository provides a flat-file structure for deploying a rewards-based vault where users can lock their tokens to earn yield.

## Features
* **Time-Based Rewards**: Rewards are calculated per block or per second for high precision.
* **Emergency Exit**: A built-in function for users to withdraw their principal in case of contract pauses (safety first).
* **Owner-Controlled Rewards**: The contract owner can fund the reward pool and adjust the reward rate.
* **OpenZeppelin Integrated**: Uses `SafeERC20` to prevent common token transfer vulnerabilities.

## Technical Flow
1. **Approve**: User approves the vault to spend their ERC-20 tokens.
2. **Stake**: User calls `stake(amount)`.
3. **Earn**: Rewards accrue based on the `rewardRate`.
4. **Claim**: User calls `getReward()` to mint or transfer earned tokens.
5. **Withdraw**: User exits the pool with their original deposit.

## License
MIT
