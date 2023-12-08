# Bibi NFT Mint Smart Contract

## Overview

The `bibi::nft_mint` module defines a smart contract on the Aptos Blockchain for minting NFTs within the exclusive Bibi collection. This contract allows users to mint unique NFTs, each associated with a specific identifier and metadata.

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
  - [Initialization](#initialization)
  - [Minting NFTs](#minting-nfts)
- [Constants](#constants)
- [Error Codes](#error-codes)
- [Structs](#structs)
- [Public Functions](#public-functions)
- [Utility Functions](#utility-functions)

## Getting Started

### Prerequisites

- Aptos Blockchain environment
- Move language compiler and runtime

### Installation

1. Deploy the smart contract on the Aptos Blockchain.
2. Ensure that the `aptos_token` and other required modules are available.

## Usage

### Initialization

The smart contract must be initialized by an administrator. This sets up the minting pool and creates the NFT collection.

```move
// Example initialization
admin_address = @bibi;
bibi::nft_mint::init(&admin_address);
