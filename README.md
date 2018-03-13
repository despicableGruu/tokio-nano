# Nano-rs
Nano-rs is a pure Rust implementation of the Nano cryptocurrency based on Tokio. It is currently in its very infancy.

This repo serves as a monorepo that contains several crates, including the root `nano-rs` crate, which is the node implementation itself. There are also several subcrates:

- `nanopow-rs` is a standalone Proof of Work implementation.
- `nano-lib-rs` provides types and functions for working with the Nano protocol in Rust.

## Milestones:
- [ ] A basic node that can validate and store blocks sent to it
  - [ ] Data structures
    - [x] Blocks
    - [x] Message headers
    - [ ] Message body
      - [x] Block
      - [ ] Keepalive peers
  - [ ] Database
  - [x] Proof of work
  - [ ] Cryptographic functions
  - [ ] Basic wallet functions
  - [ ] Networking
    - [ ] Receiving keepalives and blocks
      - [x] (partial) keepalives
      - [ ] publish
      - [ ] confirm_ack
    - [x] (partial) Sending keepalives
- [ ] Add broadcasting and discovery
- [ ] Add RPC interface
- [ ] Add voting
- [ ] Add compatibility with existing Nano Nodes
- [ ] Add complete testing harness
- [ ] Possibly more things in the future
