# Fabstir

Building the foundational infrastructure for Web3 entertainment and decentralised applications.

<p align="center">
<img src="https://fabstir.com/img2/Fabstir%20Core%20Principles%20details%20diag%20202511.jpg" width="690" alt="Fabstir overview">
</p>

## Overview

Fabstir is revolutionising the entertainment industry by enabling creators and distributors to operate truly owned, interconnected streaming platforms—replacing the 30-50% extraction model with transparent smart contracts and instant, verifiable payments. We're building collaborative networks where distributors, filmmakers, musicians, creators and consumers thrive together through enriched social experiences.

Visit our website at https://fabstir.com to learn more.

## Open-Source Contributions

### Technical Stack

Our open-source infrastructure combines cutting-edge Web3 technologies:

**Frontend:**

- Next.js, React, JavaScript, TypeScript
- Tailwind CSS, ethers.js
- WebAssembly (WASM), Rust

**Backend:**

- Node.js, Express.js
- Rust, Python
- RESTful APIs, HTTP/2

**Blockchain Infrastructure:**

- Base (Ethereum Layer-2) - Primary blockchain
- Polygon (Ethereum Layer-2) - Secondary blockchain
- Coinbase Smart Wallet - Passkey authentication
- Particle Network Wallet - Alternative wallet integration

**Decentralised Storage:**

- Sia S5 Network - Primary content delivery and storage
- IPFS - Distributed file storage and content addressing

**AI & Machine Learning:**

- Mixtral 8x7B and 8x22B LLM - Self-hosted open-source models

### Key Projects

#### Fabstir Cinema Player (Open-Source)

Successfully deployed at Karma Sanctum Soho cinema, screening award-winning short films including Oscar-nominated content. This open-source media player enables:

- Direct filmmaker-to-cinema streaming via blockchain
- 4K video playback with smooth performance
- Instant payment distribution to creators during screenings
- NFT minting capabilities for digital ownership
- [View code](https://github.com/Fabstir/Fabstir_Media_Player_Snaps)

#### Fabstir Platform Ecosystem (Mixed Open/Closed Source)

White-label streaming platforms that distributors can customise with their branding whilst joining our collaborative network:

- **Non-Multiplex Cinema Platform** - Launching September 2025 for short films and festival content
- **Magic Town** - Commercial platform for films and TV series
- Full social media integration (threads, chat, following)
- Multiple monetisation models (subscription, purchase, auction, tipping)
- Smart contract automation for revenue splits between creators and distributors
- Core infrastructure is open-source, business logic proprietary

#### Video Transcoding Infrastructure (Open-Source)

High-performance transcoding supporting both h264 (wide compatibility) and AV1 (superior compression):

- Hardware acceleration via NVidia 4000 series or Intel Arc
- Kubernetes orchestration for scalable workloads
- Optimised for S5 network performance
- Handles 4K content that distributors demand
- [View code](https://github.com/Fabstir/transcode-example) and [infrastructure](https://github.com/Fabstir/transcode-infra)

#### Smart Contract Suite (Open-Source)

Comprehensive blockchain infrastructure enabling:

- **Revenue Distribution Contracts** - Automatic splits between multiple parties
- **NFT Streaming Rights** - Limited edition digital ownership (e.g., 10,000 copies per film)
- **Collaborative Business Models** - Cross-platform licensing without lawyers
- **FAB Token System** - Tiered staking (1k-500k FAB) with creator benefits
- **DAO Governance** - Community-driven platform decisions
- Audited contracts ensuring security for millions in transactions

#### Account Abstraction & Onboarding (Open-Source)

Eliminating Web3 complexity for mainstream adoption:

- Credit/debit card payments. Now with Coinbase Smart Wallet integration
- Social login (Google, Facebook, email) creating self-custodial wallets
- Gasless transactions using Coinbase Smart Wallet for seamless UX
- No crypto knowledge required - users don't even know they're using blockchain
- [View implementation](https://github.com/Fabstir/Fabstir_Media_Player_Snaps/tree/main/packages/site)

#### Decentralised Storage Integration (Open-Source)

Deep integration with Sia's S5 network providing:

- Content-addressed storage with on-chain hash verification
- End-to-end encryption for premium content
- Cost-effective CDN alternative beating traditional infrastructure
- True data ownership - content can't be deplatformed
- Browser-based access through WebTransport

#### AI-Powered Discovery System (Closed Source)

Self-hosted Mixtral LLMs enabling:

- Cross-platform content discovery across all distributors
- Semantic search matching films to audience preferences
- Content moderation and community flagging
- Source attestation for combating deepfakes
- No vendor lock-in or per-request costs

#### WGPU 3D Rendering Engine (Open-Source)

Advanced rendering capabilities for next-generation content:

- Direct GPU hardware access via WebGPU
- Support for ERC-7401 nestable NFTs
- Complex 3D model construction and navigation
- Future-proofing for metaverse integration
- [View renderer](https://github.com/Fabstir/fabstir-renderer)

#### MetaMask Snaps Integration (Open-Source)

Extending wallet capabilities whilst maintaining security:

- Store NFT and 3D model data within wallets
- Enhanced user experience for Web3 interactions
- Secure isolated environment on host devices
- Discovery mechanism for new users
- [View implementation](https://github.com/Fabstir/Fabstir_Media_Player_Snaps)

#### AI Vector Database (Coming Soon - Open-Source)

Next-generation AI infrastructure for Web3:

- Decentralised vector storage with MCP server integration
- HAMT sharding for millions of vectors with O(log n) lookups
- Cryptographic proof of AI data sources
- Native Base smart contracts with EIP-712 signatures
- Enabling verifiable AI agents and RAG applications

### Why This Matters

We're solving Web3's biggest infrastructure problem by creating:

- ✅ Performance optimisation through decentralised storage
- ✅ Cost-effective data solutions without gatekeepers
- ✅ True data validation and integrity
- ✅ Genuine user data ownership

Our upcoming app store will serve as distribution and payment rails, allowing ANY Web3 developer to plug their applications directly into our ecosystem.

## License

Fabstir network infrastructure is open-source (MIT License). Individual Fabstir applications use a mixture of open and closed source components.

## Sia Foundation Grant: Enhanced s5.js

### Building Developer-Friendly Infrastructure

Jules Lai, Fabstir's founder, has been awarded a Sia Foundation grant to enhance the s5.js library with critical developer features that make decentralised storage accessible to mainstream developers.

**Key Enhancements Being Developed:**

1. **Path-based API** - Simple operations like `getByPath(rootKey, '/profile/settings')` and `putByPath(rootKey, '/gallery/photo.jpg', data)`

2. **Media Handling Pipeline** - Automatic thumbnail generation for images, metadata extraction, and progressive loading support

3. **Reliable Updates** - Last-Writer-Wins conflict resolution for safe concurrent writes

4. **Directory Utilities** - Efficient browsing of large collections with pagination and caching

5. **FS5 Sharding Groundwork** - HAMT/B-Tree implementations for handling massive directories

These improvements complement Sia's recent v2 hardfork capabilities (browser-based access via WebTransport, 99% reduced blockchain storage through UTreeXO) and make S5 the missing infrastructure layer that Web3 developers need.

**Why This Matters for Fabstir:**
With many US film distributors and production houses interested in onboarding, bringing potentially 1000s of films and millions of users, this grant work ensures our decentralised infrastructure can scale to meet demand whilst maintaining performance and reliability.

**Learn more about the enhanced s5.js project:** [https://github.com/julesl23/enhanced-s5js-design](https://github.com/julesl23/enhanced-s5js-design)

All enhancements will be contributed back to the upstream s5.js repository as open-source code under the MIT licence.

---

_Building the foundational infrastructure that makes truly decentralised applications viable for mainstream adoption._
