
<img src="images/logo.png" style="display: block; height: 12em; margin: 0 auto;"/>

ION is a public, permissionless, Decentralized Identifier (DID) network that implements the blockchain-agnostic Sidetree protocol on top of Multichain (as a 'Layer 2' overlay) to support DIDs/DPKI (Decentralized Public Key Infrastructure) at scale.

**IMPORTANT NOTE:** The majority of ION's code is developed under the blockchain-agnostic Sidetree protocol's repo: https://github.com/decentralized-identity/sidetree, which this project uses internally with the code required to run the protocol on Multichain, as the ION network.

## Key Points:

- ION can be operated both as a public and permissionless system but also as a private and permissioned one or even as a hybrid - certain multichain nodes may be permissionless and others permissioned.
- ION is not a sidechain or consensus system - the different blockchains may have different consensus systems as determined by the node operators.

## How does ION work?

By leveraging the blockchain-agnostic Sidetree protocol, ION makes it possible to anchor tens of thousands of DID/DPKI operations on a target chain (in ION's case, Multichain) using a single on-chain transaction. The transactions are encoded with a hash that ION nodes use to fetch, store, and replicate the hash-associated DID operation batches via IPFS. The nodes process these batches of operations in accordance with a specific set of deterministic rules that enables them to independently arrive at the correct DPKI state for IDs in the system, without requiring a separate consensus mechanism, blockchain, or sidechain. Nodes can fetch, process, and assemble DID states in parallel, allowing the aggregate capacity of nodes to run at tens of thousands of operations per second.

## Building the project:

Please use the following guide to setup the various services that comprise an ION node: [ION Installation Guide](https://github.com/decentralized-identity/ion/blob/master/install-guide.md).

## Partner Organizations:

- ION (a instantiation of Sidetree on Bitcoin) has been developed as a part of the [Decentralized Identity Foundation](https://identity.foundation/)
