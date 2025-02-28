# Go Raydium Swap

A Go-based command-line tool for performing token swaps on the Raydium DEX (Decentralized Exchange) on the Solana blockchain. This tool interacts with Raydium's API to execute token swaps with optimal pricing and transaction handling.

## Features

- Token swapping on Raydium DEX
- Automatic priority fee calculation
- Support for SOL wrapping/unwrapping
- Transaction version V0 support
- Real-time swap quote fetching
- Comprehensive error handling and logging

## Configuration

The following constants can be configured in `main.go`:

- `InputMint`: The token mint address to swap from (default: SOL)
- `OutputMint`: The token mint address to swap to (default: USDC)
- `Amount`: The amount of input tokens to swap
- `Slippage`: Slippage tolerance percentage
- `TxVersion`: Transaction version (default: "V0")
- `IsInputSol`: Whether the input token is SOL
- `IsOutputSol`: Whether the output token is SOL

## Usage

1. Place your Solana wallet private key JSON file in a secure location
2. Update the wallet path in `main.go`:
```go
keyData, err := os.ReadFile("/path/to/your/wallet.json")
```