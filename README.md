# Zero-Knowledge Payment Protocol

A privacy-preserving payment protocol using hierarchical Merkle trees and zero-knowledge proofs.

## Overview

This protocol enables private, instant, and verifiable transactions through a three-layer architecture:

```
Global Tree (Public)
   └── Wallet Trees (Private)
          └── Channel Trees (Private)
```

All state transitions are validated using zero-knowledge proofs, ensuring privacy while maintaining verifiability.

## Key Features

- **Privacy**: Transaction details known only to sender and recipient
- **Instant Settlement**: No consensus requirements for basic operations
- **Scalability**: Hierarchical Merkle trees for efficient state management
- **Trustless**: All state transitions verified through ZK proofs
- **Unilateral Updates**: No recipient confirmation required for transfers

## Documentation Structure

- `docs/architecture.md` - System architecture and components
- `docs/protocol.md` - Detailed protocol specification
- `docs/proofs.md` - Zero-knowledge proof system
- `docs/security.md` - Security analysis and guarantees

## Security Properties

The protocol guarantees:

1. **Transaction Privacy**: Only sender and recipient know transaction details
2. **Balance Privacy**: All balances kept private through commitments
3. **State Integrity**: All updates cryptographically verified
4. **Update Atomicity**: Consistent state transitions
5. **Proof Soundness**: No invalid state transitions possible

## Getting Started

See `docs/architecture.md` for a complete system overview and implementation guidelines.