# Scaffold Studio

![Scaffold Studio Banner](https://raw.githubusercontent.com/Scaffold-Studio/stellar-studio-brand-assets/main/scaffold-studio-banner.png)

**Deploy and command Stellar tokens, NFTs, and DAOs through conversation.**

No Soroban coding required. Stellar Studio is an MCP-powered platform that lets you deploy, manage, and operate tokens, NFTs, and governance contracts using natural language.

**Live at [scaffold-studio.app](https://scaffold-studio.app)**
• **GitHub:** [github.com/Scaffold-Studio](https://github.com/Scaffold-Studio)
• **X (Twitter):** [@scaffold_studio](https://x.com/scaffold_studio)

**AI copilots for Stellar builders.**

## About

**80+ tools. 5 contract types. Zero Soroban code.**

Deploying Soroban smart contracts usually requires writing Rust, understanding complex SDKs, and navigating deployment tooling. Stellar Studio eliminates all of that - just describe what contract you want to deploy, and we handle the rest through the Model Context Protocol.

**What we've built:**
- **80+ blockchain operation tools** - Deploy, mint, transfer, burn, approve, vote, and more
- **5 smart contract types** - Tokens (Pausable, Capped, Allowlist, Blocklist, Vault), NFTs (Enumerable, AccessControl), Governance (MerkleVoting)
- **Factory pattern deployment** - Standardized, audited contracts deployed through factory contracts
- **MCP server integration** - Works with Claude Desktop, Cursor, VS Code through Model Context Protocol
- **Production ready** - All contracts tested and deployed on Stellar testnet

## Why Stellar Studio

- **No Soroban Coding**: Deploy smart contracts without writing a single line of Rust
- **Natural Language**: Just say "deploy a token named MyToken" and it happens
- **Multiple Interfaces**: Use Claude Desktop, Cursor IDE, VS Code, or our web interface
- **Type-Safe**: MCP server built with TypeScript, contracts built with Rust
- **Open Source**: All code, contracts, and tools are fully open source

## Tools

Deploy and manage:
- **Tokens**: Pausable, Capped, Allowlist, Blocklist, Vault tokens
- **NFTs**: Enumerable and AccessControl collections
- **Governance**: MerkleVoting with privacy-preserving proofs
- **Registry**: Publish and version your contracts
- **Utilities**: Merkle trees, validation, configuration builders

## Projects

### [Stellar-Studio-MCP](https://github.com/Scaffold-Studio/Stellar-Studio-MCP)
Model Context Protocol server that powers AI-blockchain interactions. Features 80+ tools for comprehensive Stellar Soroban operations including:
- Smart contract deployment (Token, NFT, Governance factories)
- Contract operations (transfer, mint, burn, approve, vote)
- Registry integration (publish, deploy, version management)
- Utility functions (merkle trees, validation, builders)
- Network support (local, testnet, mainnet)

### [Stellar-Studio-Contracts](https://github.com/Scaffold-Studio/Stellar-Studio-Contracts)
Production-ready Soroban smart contracts powering the ecosystem:
- Factory contracts (MasterFactory, TokenFactory, NFTFactory, GovernanceFactory)
- Token templates (Pausable, Capped, Allowlist, Blocklist, Vault)
- NFT templates (Enumerable, AccessControl, Royalties)
- Governance contracts (MerkleVoting)
- All contracts optimized and deployed on testnet

### [Stellar-Studio-Frontend](https://github.com/Scaffold-Studio/Stellar-Studio-Frontend)
Web interface for Scaffold Studio providing visual contract deployment and blockchain interaction tools powered by AI.

## Quick Start

```bash
# Clone and setup MCP server
git clone https://github.com/Scaffold-Studio/Stellar-Studio-MCP
cd Stellar-Studio-MCP
pnpm install && pnpm build

# Configure environment
cp .env.testnet .env
# Edit .env with your Stellar secret key

# Automated setup for your AI application
pnpm setup:claude  # or setup:cursor, setup:code
```

## Example Deployments

Natural language contract deployment:

- **"Deploy a token named MyToken with symbol MTK"** → Token contract deployed via TokenFactory
- **"Create an NFT collection called CoolNFTs"** → NFT contract deployed and ready to mint
- **"Deploy governance with these voter addresses"** → MerkleVoting contract with cryptographic proofs
- **"Transfer 1000 MTK tokens to address GA..."** → Execute token transfer operation
- **"Mint 10 NFTs to my address"** → Batch mint NFTs from your collection
- **"Publish my WASM to the registry"** → Version and publish compiled contracts

## Technology Stack

- **Model Context Protocol**: Standard for AI-tool integration
- **Stellar SDK**: Official Soroban smart contract libraries
- **TypeScript**: Type-safe development with modern tooling
- **Rust**: High-performance smart contracts
- **Plugin Architecture**: Modular and extensible design

## Architecture

```
┌─────────────────────────────────────────────────────────┐
│                   AI Clients Layer                      │
│         Claude Desktop • Cursor • VS Code               │
└─────────────────────────────────────────────────────────┘
                           │
                           ▼
┌─────────────────────────────────────────────────────────┐
│              MCP Server (80+ Tools)                     │
│   Factory • Token • NFT • Governance • Registry         │
└─────────────────────────────────────────────────────────┘
                           │
                           ▼
┌─────────────────────────────────────────────────────────┐
│           Stellar Soroban Network                       │
│    TokenFactory • NFTFactory • GovernanceFactory        │
└─────────────────────────────────────────────────────────┘
```

**Get Started**: Try it live at [scaffold-studio.app](https://scaffold-studio.app) or explore our [MCP Server](https://github.com/Scaffold-Studio/Stellar-Studio-MCP) to deploy and command Stellar tokens, NFTs, and DAOs through conversation.

---

**Scaffold Studio** — Deploy and command Stellar tokens, NFTs, and DAOs through conversation.

Visit us at [scaffold-studio.app](https://scaffold-studio.app)
