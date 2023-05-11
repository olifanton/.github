Olifanton 💎
---

<p align="center">
  <a href="https://github.com/olifanton"><img align="center" width="864" src="https://github.com/olifanton/.github/blob/main/profile/olifanton_banner.png" /></a>
</p>

_Olifanton_ is a set of libraries and PHP SDK for working with **The Open Network (_TON_)**

## Installation

```bash
composer require olifanton/ton
```

For additional information see [`olifanton/ton`](https://github.com/olifanton/ton) repository.

## 🛠️ SDK components

- [X] Mnemonics [🔗](https://github.com/olifanton/mnemonic)
  - [X] Generation
  - [X] Validation
- [X] Address [🔗](https://github.com/olifanton/interop#address)
- [X] BoC
  - [X] Cell [🔗](https://github.com/olifanton/interop#cell)
  - [X] Slice [🔗](https://github.com/olifanton/interop#slice)
  - [X] Cell builder [🔗](https://github.com/olifanton/interop#builder)
  - [X] Hashmap [🔗](https://github.com/olifanton/interop#hashmap)
- [X] Blockchain transport
  - [X] Message signing
  - [X] Toncenter client [🔗](https://github.com/olifanton/ton#toncenter-transport-initialization)
- [X] DNS client
- [X] Smart-contracts
  - [X] Wallets
    - HighloadV2
    - Simple, V2, V3
    - V4 with plugins methods
  - [X] Jettons
    - [X] Minter
    - [X] Wallet
  - [X] NFT
    - [X] Collection
    - [X] Item
- [X] Helpers
  - [X] Metadata helpers
  - [X] Deployer

## 🚧 In progress

- [ ] `tonlibjson` transport via FFI [🔗](https://github.com/olifanton/tonlibjson-transport)

## 💡 Planned roadmap

- [ ] On-chain and semi-chain metadata
- [ ] Payment channels
- [ ] SBT
- [ ] TON Connect 2.0
- [ ] Additional BoC features
  - [ ] Tuples
  - [ ] Merkle proofs
