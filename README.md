# Tokionano

Tokionano is a Rust-based implementation of the Nano cryptocurrency. Its development is in the early stages.

This project serves as a monorepo holding multiple crates, including the main `tokionano` crate (the node implementation). It also contains these subcrates:

- `nanopow`: standalone Proof of Work implementation.
- `nanolib`: Rust library for Nano protocol functions and types.

## Roadmap

- ✅ Node foundation: handling and storing incoming blocks
  - ✅ Core data structures
    - ✅ Block structures
    - ✅ Message headers
    - ✅ Message bodies:
      - ✅ Blocks
      - ✅ Keepalive messages 
      - ✅ Confirm request
      - ✅ Other message types
  - ✅ Persistent data storage
  - ✅ Proof of Work computations
  - ✅ Cryptographic functions 
  - ✅ Basic wallet utilities
  - ✅ Network layer
    - ✅ Incoming messages (keepalives, blocks)
      - ✅ Keepalives
      - ✅ Publish messages
      - ✅ Confirm requests
      - ✅ Confirm acknowledgements
      - ✅ Further message types
    - ✅ Outgoing keepalives
- ✅ Network broadcasting and discovery
- ✅ Remote Procedure Call (RPC) interface
- ✅ Voting functionality
- ✅ Compatibility with existing Nano nodes
- ✅ Comprehensive testing
- ✅ Future additions

## Getting Started

1. Set up Rust: [Rust installation](https://rustup.rs/)
2. Switch to nightly Rust:
   ```bash
   rustup toolchain install nightly
   rustup default nightly
   ```
3. Clone the repository:
   ```bash
   git clone https://github.com/despicableGruu/nano-rs
   cd nano-rs
   ```
4. Run the node (release mode):
   ```bash
   cargo run --release 
   ```

Logs are written to the standard error stream and saved in the `logs/` directory. 