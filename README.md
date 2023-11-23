# .github

This is the official GitHub repository of Fabstir, a builder of innovative solutions for Web3 and AI. Our projects include full-stack web3 development, decentralised peer-to-peer technology, video streaming, 3d rendering, and more. Visit our website at https://fabstir.com to learn more about us and our work.

<img src="https://github.com/Fabstir/.github/blob/main/Fabstir_github.png" width="690" width="540" alt="Fabstir overview">

## Introduction

Fabstir has built an open-source Web3 layer that utilises Sia's decentralised storage.

# Overview

## Tokenisation

Property rights stored on public EVN compatible blockchain that hold immutable accounts with off-chain data held on [Sia](https://sia.tech/) peer-to-peer decentralised network via [S5](https://github.com/s5-dev/S5). S5’s content-addressed data ensures that hashes stored on the blockchain verifies the data integrity of the off-line storage. This ensures content creators keep the IP they create whether that be images, video, audio, text, files, code, 3d models, contracts, NFT metadata and more all stored on Sia through S5 via [client](https://github.com/parajbs-dev/s5client-js) Javascript SDK. Modern encryption of the assets' data ensure that creators have complete ownership and control through their digital wallet. Fabstir is implementing standards from [NFT 2.0](https://singular.app/) (now called modular NFTs). Code [here](https://github.com/Fabstir/Fabstir_Media_Player_Snaps/tree/main/packages/site)

## Video Transcoder

Transcodes videos into h264 and AV1 format. H264 format ensures compatibility with most devices or browsers. AV1 is a more modern codec that offers much better compression ratio, higher quality and is license free to use. Produced videos then can play smoothly using S5 network.
AV1 requires complex computation to transcode, hence GPU hardware with transcoding hardware built-in such as NVidia 4000 series of graphics cards or Intel Arc. Code [here](https://github.com/Fabstir/transcode)

## Account Abstraction

A major reason why there has not been mass adoption of Web3 dapps that can counter equivalent Web2 apps is that the onboarding process is difficult and cumbersome. Now with account abstraction, gas fees can be paid with the same token as the transaction itself. This removes the need to hold native blockchain tokens separate from the currency used in the transactions. For example, an ERC-20 stablecoin can be used throughout now. This works because user accounts are in this case addresses of smart contracts (computer code) to enable the extra functionality. Fabstir is working with [Biconomy](https://www.biconomy.io/) for its account abstraction implementation. Code [here](https://github.com/Fabstir/Fabstir_Media_Player_Snaps/tree/main/packages/site)

## Social Login

Advancement in digital wallets, means that many allow for payment with debit/credit or bank account for digital currency straight from the wallet. Users can login with their social media account or email, removing friction from the onboard process to Web3, and by default, users receive their crypto account (smart contract account) that by default gives them self-custody of digital assets and currencies. Users can learn this fact at their own pace and not immediately faced with the technicals. Fabstir is working with [Particle Network](https://particle.network/) for its wallet integration with social login. Code [here](https://github.com/Fabstir/Fabstir_Media_Player_Snaps/tree/main/packages/site)

## Snaps

[Metamask Snaps](https://metamask.io/snaps/) is a framework for extending the capabilities of the Metamask wallet, stores its state in an isolated environment on the host device. This design decision is made for enhanced security and privacy.
This allows many different types of data to be stored in the wallet, not just tokens and balances.
Fabstir stores in Metamask snaps state NFT data, 3d model data and video links. Code [here](https://github.com/Fabstir/Fabstir_Media_Player_Snaps/tree/main)

## WGPU

Is the successor to WebGL and boasts much faster rendering times. This is because [WebGPU](https://www.w3.org/TR/webgpu/) has more direct hardware access to the GPU. It also supports compute shaders, Vulkan and DirectX APIs to offload much more work to the GPU.
Fabstir uses [WGPU](https://github.com/gfx-rs/wgpu) (a Rust wrapper to WebGPU), to enable 3d models to be rendered with direct lighting and textures. Each 3d model is an NFT whose metadata stores the 3d data in .gltf or .obj files. As Fabstir’s implementation supports ERC-7401 nestable NFTs, much larger 3d models can be built up from composing together smaller NFT 3d models. Navigation controls allow the user to fly around in their created models. Code [here](https://github.com/Fabstir/fabstir-renderer)

## Kubernetes

[Kubernetes](https://kubernetes.io/) (also known as K8s) is an open-source container orchestration platform that automates many of the manual processes involved in deploying, managing, and scaling containerized applications. Deployment can be done on a variety of platforms, including on-premises, hybrid, and public cloud infrastructure. The video/audio transcoder was written to use Kubernetes as transcoding workloads can be quite high and if used by a lot of users, Kubernetes is able to scale up to recruit more computers to handle the increased workload and scale down when workload subsides. Code [here](https://github.com/Fabstir/transcode-infra-example)
