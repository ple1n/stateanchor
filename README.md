
# State*Anchor*

Lightweight post-quantum blockchain built upon recursive STARK proofs that is not nosiy.

Like [Mina](https://docs.minaprotocol.com/mina-protocol), it produces a constant-sized proof, but written in ZKVM and quantum-proof.

The chain is transport agnostic. It's written as a state machine running on [Freenet](https://github.com/freenet/freenet-core/). 

This is a Proof of Stake network where stakes are backed by on-chain currency, and external assets, such as contracts on other chains.

The voting majority will eventually produce the longest chain, where the forks, when reaching a certain threshold, cause a slash of stakes that transfer funds to the rest of voting members and the whistleblower. 

For assets backed by contracts on other chains, the transfer is trustless, through a ZK proof of *excessive forking*.

## Fully private and succint

We name it _StateAnchor_, because it does not intend to serve data. Rather, it serves as an anchor of data. The chain presents itself as a perpetually updating state root hash, with a recursive STARK proof that itself proves the entire chain state trustlessly. 

Miners transmit minimal data to keep the chain working. Succintness is the goal, while being private is almost a side product.

## Currency, redefined

Is currency just money, or more or less a representation of reputation in a community. 

We don't charge flat fees for transactions and contract creation. The limited resources are supposed to serve the community. No more transaction spam. 

> **Public goods are good.**  
> — *Vitalik Buterin*


## Interop, not compete

We don't intend to be the next 'winner chain'. Smaller chains can peg stakes onto mature chains to harden consensus. Assets can be transferred easily across chains thanks to contracts and ZK state proofs.

## Minimal, to serve Web3

The chain is designed from ground-up to serve the needs for daily internet protocols such as apps that run on Freenet. 

This project shall be minimal, and perhaps work as a proof-of-concept, as [Mel](https://melproject.org/en/) advocated.

### Offline-first consensus

The economic protocol is designed such that, a single state proof including only one branch is enough to attest to the validity of consensus, because if you can provide a _proof of excessive forking_, you can slash funds. 

This can be incredibly useful for real world applications. We don't want users to be constantly syncing from the network, getting new updates every 10 minutes, just to make sure they aren't fooled by false claims, even if its a fixed size proof. 

In a censorship ridden environment, constant syncing creates identifiable traffic pattern, harming user privacy. 

see more in [draft](./spec.typ)

### More secure than root CAs

It can serve as a new backbone of Publickey Infrastructure, such that unique names can not be hijacked by attackers. Trust nobody but a single STARK proof.

## Centralized, for the decentralized web

It may seem centralized as you see how the currency works. Fear not, it's a manipulation into the fabric of money which eventually serves our goals. 

Men are inevitably constrained by the machinery of society. Only through re-engineering the machinery can we be free.