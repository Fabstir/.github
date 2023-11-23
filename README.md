# .github

This is the official GitHub repository of Fabstir, a builder of innovative solutions for Web3 and AI. Our projects include full-stack web3 development, decentralised peer-to-peer technology, video streaming, 3d rendering, and more. Visit our website at https://fabstir.com to learn more about us and our work.

<p align="center">
<img src="https://github.com/Fabstir/.github/blob/main/Fabstir_github.png" width="690" width="540" alt="Fabstir overview">
</p>

## Summary of Open-Source Contributions by Fabstir in Web3 Technology

### Introduction

Fabstir's development can be thought of as an open-source layer atop Sia storage, incorporating the features of Web3.

### Fabstir: The Web3 Layer

#### Tokenisation

Fabstir utilises a public EVM-compatible blockchain for storing property rights. These immutable accounts are complemented with off-chain data hosted on the peer-to-peer decentralised network of [Sia](https://sia.tech/) through [S5](https://github.com/s5-dev/S5). S5’s content-addressing hashes that are kept on the blockchain then authenticate the data integrity of offline storage. This approach safeguards intellectual property for creators of diverse content types (whether that be images, video, audio, text, files, code, 3d models, contracts, NFT metadata and more), all stored on Sia via S5 using a [JavaScript client SDK](https://github.com/parajbs-dev/s5client-js). Additionally, Fabstir adopts standards from [Modular NFTs](https://singular.app/) (formerly NFT 2.0) to ensure modern encryption and comprehensive ownership control through digital wallets. Further details and code are available [here](https://github.com/Fabstir/Fabstir_Media_Player_Snaps/tree/main/packages/site).

#### Video Transcoder

The transcoder supports h264 and AV1 formats. While h264 ensures wide compatibility, AV1 offers improved compression and quality without licensing fees. Optimal performance on the S5 network is achieved through hardware like NVidia 4000 series graphics cards or Intel Arc for AV1 transcoding. Code can be found [here](https://github.com/Fabstir/transcode).

#### Account Abstraction

To streamline Web3 dapp adoption, Fabstir utilises account abstraction. This eliminates the need for separate native blockchain tokens, allowing transactions and gas fees to be paid with the same token, like an ERC-20 stablecoin. This is made possible by treating user accounts as smart contract addresses. Fabstir’s collaboration with [Biconomy](https://www.biconomy.io/) is crucial for this implementation. More information and code is available [here](https://github.com/Fabstir/Fabstir_Media_Player_Snaps/tree/main/packages/site).

#### Social Login

Fabstir’s dapps now support direct payments from debit/credit cards or bank accounts. Users can log in with their social media accounts or email, seamlessly integrating into the Web3 ecosystem with a self-custodial crypto account. This user-friendly approach is facilitated by our partnership with [Particle Network](https://particle.network/), and further details and code are provided [here](https://github.com/Fabstir/Fabstir_Media_Player_Snaps/tree/main/packages/site).

#### Snaps

Through the [Metamask Snaps](https://metamask.io/snaps/) framework, Fabstir extends Metamask wallet capabilities while maintaining a secure, isolated environment on the host device. This enables storage of various data types, including NFT and 3d model data, within the wallet. More information and code is available [here](https://github.com/Fabstir/Fabstir_Media_Player_Snaps/tree/main).

#### WGPU

Fabstir employs [WGPU](https://github.com/gfx-rs/wgpu), a Rust wrapper for [WebGPU](https://www.w3.org/TR/webgpu/), offering superior rendering speeds and direct GPU hardware access. Our implementation supports ERC-7401 nestable NFTs for constructing intricate 3d models, with navigation controls to view from different angles. Additional details and code can be found [here](https://github.com/Fabstir/fabstir-renderer).

#### Kubernetes

Utilising [Kubernetes](https://kubernetes.io/), Fabstir efficiently manages high workloads in video/audio transcoding, with scalable deployment options across various platforms. This infrastructure is critical for meeting user demand fluctuations. Further details and code are available [here](https://github.com/Fabstir/transcode-infra).
