# Amin Talebi

Backend and protocol engineer in Berlin. I work in Go and Rust on distributed systems and blockchain protocols, and these days mostly on zero-knowledge proof systems.

I'm open to senior engineering roles.

[Website](https://amintalebi.com) · [LinkedIn](https://linkedin.com/in/amintalebi) · [Email](mailto:talebi242@gmail.com)

## Open source

### [openvm-poseidon2](https://github.com/amintalebi/openvm-poseidon2)

`Rust` `OpenVM` `Plonky3` `RISC-V`

A Poseidon2 extension for the [OpenVM](https://github.com/openvm-org/openvm) zkVM.

Without it, a guest program that needs Poseidon2 has to build the hash out of RISC-V arithmetic: thousands of instructions, each one proved. With it, one permutation is one custom instruction.

- **Instruction:** `PERMUTE` permutes a 16-word state in memory, in place.
- **Circuit:** a permute chip reads and writes the state, and a periphery chip proves the output is the permutation of the input. Both are AIRs over BabyBear, connected by a lookup bus.
- **Guest library:** a sponge hasher plus `hash_u32s`, `hash_bytes` and the raw `permute`.
- **Example:** builds, executes, proves and verifies a guest program through the SDK.

It is still in development and has not been audited.

### Contributions

- **[ethereum/go-ethereum#27845](https://github.com/ethereum/go-ethereum/pull/27845)** (Go). Added state overrides to `eth_estimateGas` in Geth, so a caller can estimate gas against modified balances, code and storage.
- **[safe-global/safe-modules-deployments#150](https://github.com/safe-global/safe-modules-deployments/pull/150)** (TypeScript). Added the Social Recovery Module deployment on Arbitrum One.
- **[zarbanio/subgraph](https://github.com/zarbanio/subgraph)**. (TypeScript) The subgraph for the Zarban stablecoin protocol.
- **[SOFIE-project/Marketplace](https://github.com/SOFIE-project/Marketplace)** (Solidity, Python). Ethereum smart contracts and a web3 client for an on-chain marketplace, written at Aalto University.

### Older projects

- **[paxos](https://github.com/amintalebi/paxos)** (Python). An implementation of the Paxos consensus algorithm.

## Where I've worked

- **[Delivery Hero](https://media-solutions.deliveryhero.com/advertising-solutions/)**: display ad server
- **[Talon.One](https://docs.talon.one/docs/product/applications/manage-campaign-evaluation#create-a-campaign-evaluation-group)** (acquired by Adyen): promotion engine
- **[Zarban](https://zarban.io/)**: stablecoin protocol, as founding engineer
- **[Snapp](https://snapp.ir)**: real-time messaging
- **Aalto University**: SOFIE project

The details are on [my website](https://amintalebi.com).
