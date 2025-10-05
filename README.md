<div align="center">
  <img src="public/images/logo.png" alt="N.OVA Logo" width="120"/>
  
  # N.OVA
  
  **AI-Native Identity Platform for Web3**
  
  Transform your wallet data into a living, expressive digital identity
  
  [Live Demo](https://nova-ai.vercel.app) • [Watch Video](https://www.youtube.com/watch?v=aQttf04cBU4)
  
</div>

---

## Overview

N.OVA is an AI-powered platform built on Solana that transforms blockchain data into personalized, expressive identities. Through a comprehensive suite of generative tools including natural language chat, AI-composed music, dynamic identity cards, and on-chain analytics, N.OVA creates a unique experience around each user's blockchain behavior.

### The Problem

Modern Web3 platforms surface balances and transaction logs but fail to translate them into meaningful insights. Wallets are rich in data but void of identity, expression, or behavior-driven narrative. General-purpose LLMs such as ChatGPT, Claude, and Gemini, though powerful, are not trained to reason about on-chain activity or token structures and cannot safely explain smart contracts or interpret decentralized interactions.

### The Solution

N.OVA addresses this gap by combining purpose-built AI tooling with blockchain-native data, introducing the first modular AI identity system designed specifically for Web3 users.

---

## Core Features

### Wallet Integration
- Support for standard wallets: Phantom, Solflare, and Brave
- Smart wallet abstraction via LazorKit SDK
- Passkey-based authentication with no extensions required
- Gasless transactions for seamless user experience

### N.CHATBOT - AI Chat Assistant
- LLaMA3-based conversational AI running on Groq infrastructure
- Intelligent wallet summarization with transaction interpretation
- Smart contract analysis for Solidity and Rust files
- Token safety scanning with risk assessment
- Identification of potential vulnerabilities including mint authority and blacklist functions

### N.AURORA - Generative Music Platform
- AI-generated soundtracks personalized to wallet behavior
- Multiple mood profiles: cinematic, lo-fi, and glitch
- Dynamic evolution based on user activity
- On-demand remixing and regeneration capabilities

### Visual Identity System
- Unique AI-generated identity cards using Stable Diffusion
- Achievement-based badge system
- Progressive rank hierarchy: Echo, Pulse, Signal, Cipher, Nexus, Oracle, Sovereign
- Shareable profile exports with embedded media

### Platform Tools
- Daily token faucet: claim 10 $N.OVA tokens
- Devnet swap interface for SPL token exchanges
- Token transfer functionality
- DAO governance interface for proposal submission and voting

- Composes a custom AI-generated soundtrack based on user wallet behavior
- Tracks are mood-personalized (cinematic, lo-fi, glitch) and evolve over time
- Users can remix and regenerate tracks on demand

### Visual Identity Card

- AI-generated image (via Stable Diffusion) unique to each user
- Badge system based on behavioral milestones
- Rank progression: Echo → Pulse → Signal → Cipher → Nexus → Oracle → Sovereign

### Platform Utilities

- Faucet: claim 10 $N.OVA daily
- Devnet swap UI (SPL token ↔ $NOVA)
- Transfer SPL tokens to others
- DAO mock interface to propose/vote on features

### Dashboard & Profile

- Real-time NFT/token viewer (via Helius)
- AI chat memory and transaction timeline
- XP tracker and badge progression
- Profile export/sharing module (with embedded card and music)

---

## Technical Architecture

```
Frontend          Next.js 14 with TypeScript, TailwindCSS, Framer Motion
Wallet Layer      Solana Wallet Adapter, LazorKit SDK
AI Engine         Groq API with LLaMA3 models
Image Generation  Stable Diffusion via Replicate
Music Generation  MusicGen API
Data Storage      Supabase (user data, XP, profile memory)
Blockchain Data   Helius API (on-chain wallet analysis)
Network           Solana Devnet with SPL Token Program
```

---

## Getting Started

### Prerequisites

- Node.js version 18 or higher
- Git
- A Solana wallet (Phantom recommended) or biometric device for passkey authentication

### Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/Panacea2005/NOVA
cd NOVA
npm install
```

### Configuration

Copy the environment template and configure your API keys:

```bash
cp .env.example .env.local
```

Add the following environment variables to `.env.local`:

```env
# AI Services
NEXT_PUBLIC_GROQ_API_KEY=your_groq_api_key

# Blockchain Services
NEXT_PUBLIC_HELIUS_API_KEY=your_helius_api_key
NEXT_PUBLIC_SOLANA_MAINNET_RPC_URL=https://api.mainnet-beta.solana.com

# Image Generation
NEXT_STABILITY_API_KEY=your_stability_api_key

# Music Generation
NEXT_PUBLIC_MUSIC_API_KEY=your_music_api_key
NEXT_PUBLIC_MUSIC_AI_API_URL=https://apibox.erweima.ai/api/v1

# Database
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_key

# Additional Services
HELIUS_API_KEY=your_helius_api_key
TWITTER_API_KEY=your_twitter_api_key
NEXT_PUBLIC_API_URL=http://localhost:5000/api
NEXT_PUBLIC_CRYPTOPANIC_API_KEY=your_cryptopanic_key
```

### Development

Start the development server:

```bash
npm run dev
```

Access the application at `http://localhost:3000`

---

## Technology Stack

- Groq – ultra-fast LLM inference  
- LLaMA3 – advanced open-source LLM  
- LazorKit – passkey smart wallet abstraction  
- Supabase – real-time DB for XP/memory  
- Helius – Solana wallet analysis  
- Suno AI – AI audio synthesis  
- Stable Diffusion – hosted AI image generation

---

## Team

This project was developed by a team of three engineers for the Colosseum Breakout Hackathon 2024.

| Name  | Role |
|-------|------|
| Thien | AI Engineer and Frontend Developer |
| Anh   | AI Engineer |
| Huyen | Blockchain Specialist |

---

## License

This project is open source and available under the MIT License.

---

## Acknowledgments

We extend our gratitude to the following organizations and projects:

- Groq for providing ultra-fast LLM inference infrastructure
- LazorKit for pioneering passkey-based wallet technology
- Replicate for accessible AI model deployment
- Solana Foundation for blockchain infrastructure and developer resources
- Helius for comprehensive blockchain data APIs

---

## Contact

For questions, feedback, or collaboration opportunities, please open an issue on this repository or reach out to the team.

---

<div align="center">
  
  **Web3 identity doesn't end with what you hold — it begins with what you become.**
  
  Built with precision and purpose by the N.OVA team.
  
</div>
