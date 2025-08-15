
# StateAnchor

Lightweight blockchain built upon recursive STARK proofs that is not nosiy.

Like [Mina](https://docs.minaprotocol.com/mina-protocol), but written in ZKVM and quantum-proof.

The chain is transport agnostic. It's written as a state machine running on [Freenet](https://github.com/freenet/freenet-core/). 

This is a Proof of Stake network where stakes are backed by on-chain currency, and external assets, such as contracts on other chains. 

The voting majority will eventually produce the longest chain, where the forks, when reaching a certain threshold, cause a slash of stakes that transfer funds to the rest of voting members and the whistleblower. 

For assets backed by contracts on other chains, the transfer is trustless, through a ZK proof of *excessive forking*.

