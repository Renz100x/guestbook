# Stellar Notes DApp

**Stellar Notes DApp** - Blockchain-Based Decentralized Note-Taking System

## Project Description

Stellar Notes DApp is a decentralized smart contract solution built on the Stellar blockchain using Soroban SDK. It provides a secure, immutable platform for managing personal notes directly on the blockchain. The contract ensures that your data is stored transparently and is only manageable through predefined smart contract functions, eliminating reliance on centralized database providers.

The system allows users to create, view, and delete notes, leveraging the efficiency and security of the Stellar network. Each note is uniquely identified and stored within the contract's instance storage, ensuring data persistence and reliability.

## Project Vision

Our vision is to revolutionize personal productivity in the digital age by:

- **Decentralizing Data**: Moving note-taking from centralized servers to a global, distributed blockchain
- **Ensuring Ownership**: Empowering users to have complete control and ownership over their digital thoughts and information
- **Guaranteeing Immutability**: Providing a permanent, tamper-proof record of notes that cannot be altered or deleted by third parties
- **Enhancing Privacy**: Leveraging blockchain security to protect personal information from unauthorized access
- **Building Trustless Systems**: Creating a platform where data integrity is guaranteed by code, not by company promises

We envision a future where digital information is truly personal and sovereign, empowering individuals with complete autonomy over their digital assets.

## Key Features

### 1. **Smart Contract Custom Errors & Validation**
- Prevents invalid submissions using custom error codes: `EmptyMessage`, `MessageTooLong`, and `MaxEntriesReached`.
- Verified with unit tests using Soroban SDK test suite.

### 2. **Multi-Wallet Frontend Integration**
- Connects directly to **Freighter Wallet**.
- Real-time transaction feedback (Loading, Success, and Error state indicators).
- Live UI event updates upon new message or note creation.

### 3. **Simple Note & Guestbook Creation**
- Create notes/messages with a single function call.
- Automated ID generation for unique identification.
- Persistent storage on the Stellar blockchain.

### 4. **Efficient Data Retrieval & Security**
- Fetch all stored entries in a single call.
- View all activities directly on the blockchain with immutable records.
- Protected against unauthorized modifications.

---

## Contract Details

- **Network:** Stellar Testnet
- **Contract Address:** `CA33PZJTJZJVZ2KJ2Z6YOZNG5FBXHQQ3NZB7JVK2WEKMXCWN42LPNJP4`

---

## Technical Requirements

- Soroban SDK
- Rust programming language
- Stellar blockchain network (Testnet)
- Freighter Wallet Extension

## Getting Started

### 1. Running Unit Tests
Execute the contract tests to verify custom error handling:
```bash
cargo test