# 🔄 Solana Token Swap Program

A decentralized token swap system built on Solana, enabling direct peer-to-peer token exchanges without intermediaries or fees.

## 🌟 Features

- Direct P2P token swaps
- No intermediaries or fees
- Secure escrow mechanism
- Support for any SPL tokens

## 🧠 How It Works

1. Alice creates an offer to swap Token A for Token B
2. Bob accepts the offer, exchanging his Token B for Alice's Token A
3. The smart contract ensures a secure, atomic swap

## 🏗️ Contract Structure

- `lib.rs`: Main module and instruction handlers
- `instructions/`: Offer creation and execution logic
- `state/`: Offer state management
- `error.rs`: Custom error types
- `constants.rs`: Program constants

## 🔑 Key Processes

### Making an Offer
- Alice initiates a swap offer
- Contract creates an escrow vault
- Alice's tokens are locked in the vault
- Offer details are saved on-chain

### Taking an Offer
- Bob accepts an existing offer
- Bob's tokens are sent to Alice
- Alice's tokens are released to Bob
- Offer is closed and vault is emptied

## 🚀 Benefits

- Trustless: No third-party involvement
- Efficient: Direct swaps
- Cost-effective: No fees (only network costs)
- Flexible: Compatible with all SPL tokens

## 🛠️ Technical Stack

- Anchor framework
- Solana Program Library (SPL)
- Program Derived Addresses (PDAs) for secure vaults

---

Swap tokens securely and efficiently on Solana! 🎉
