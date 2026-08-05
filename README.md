<div align="center">

# Hi, I'm Nguyễn Quang Được (Pyro) 👋

**Full-stack game developer · Hà Nội, Việt Nam**

*I build real-time multiplayer games end to end — the client, the authoritative server, the money<br>math, and the infrastructure they run on. Right now the currency is real on-chain Bitcoin-L2<br>tokens, which makes correctness a security problem. Increasingly, so are the AI systems around it.*

<a href="https://pyrotheum1702.com/"><img src="https://img.shields.io/badge/Portfolio-pyrotheum1702.com-FF6B35?style=for-the-badge&logo=firefoxbrowser&logoColor=white" alt="Portfolio"></a>
<a href="mailto:pyrotheum1702@gmail.com"><img src="https://img.shields.io/badge/Email-pyrotheum1702%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>

</div>

---

## 🎰 Building now — Archade

A real-money instant-win game suite on **Arch Network** (Bitcoin L2). Three games — **Crazy Wheel** (real-time multiplayer betting wheel), **Deal or No Deal**, **Scratch Cards** — share one wallet and custody layer. The balance is real on-chain aUSD/aBTC, not points. I own all three tiers:

- **Clients** — Cocos Creator 2.4.13, plus a full web rewrite in **Vite + React 18 + TypeScript (strict) + Phaser 3**, hosted in a Windows XP–themed desktop shell: draggable/resizable windows, taskbar, XP dialogs.
- **Server** — Express REST + **Colyseus** realtime, MongoDB with Redis as a write-behind cache. Config is zod-validated at boot so a bad secret fails the process instead of failing later inside a money path.
- **Money** — custody wallet, one-click wallet-signed deposits (**BIP-322** via UniSat / Xverse / OKX), Telegram-approved withdrawals, an on-chain portfolio (BTC / Runes / Ordinals / Arch tokens). Amounts are integer base units end to end — converted to whole tokens only for display, at the edge.
- **Chain** — proved deposit and withdrawal against mainnet over **100 legs with zero drift** before a line of it touched the game. Along the way I reverse-engineered Arch's associated-token-address derivation — the SDK's helper derives the *wrong* address, because the chain omits Solana's `ProgramDerivedAddress` marker — and byte-verified my replacement against a live on-chain ATA.

## 🤖 AI engineering

Documented publicly in **[learning-ai-engineering](https://github.com/Pyrotheum1702/learning-ai-engineering)** — code hand-written, AI used as a tutor.

- **[PyroBot](https://github.com/Pyrotheum1702/pyro-chat-bot)** — an agentic-RAG assistant embedded on my portfolio. FastAPI + LangChain + Chroma + Fireworks, with a hand-written streaming tool-calling loop (SSE), four production tools, prompt-injection defenses, SSRF/path-traversal guards, rate limiting, and a daily LLM cost-cap kill switch. Dockerized and deployed.
- **Play Planning OS** *(client engagement)* — an agentic planning layer over a fifteen-year, ~4,400-document curriculum archive. It retrieves genuine precedent from the client's *own* archive, drafts in their measured house voice, **hard-blocks** any draft failing one of 9 safety rules, requires a human to approve — with a permanently recorded written reason to override a hard rule — and renders to 7 formats across 3 audiences. Anthropic + Voyage + Fireworks; ingestion idempotent by content hash, so it resumes for free.
- **Pyro AI Agent** — a personal discipline agent living on my VPS. Tracks GitHub and LeetCode activity plus self-reported habits, nudges over Telegram, and *infers sleep from silence* — trusting silence only while it stays uninterrupted, since any late-night activity is evidence you were awake. Inferred records are flagged so the reasoning stays auditable.
- **RAG in production games** — an in-game AI guide on a Qdrant retrieval pipeline, with a provider-agnostic LLM client and function calling.

## 🎮 Track record

7+ shipped titles — poker, slots, spin-wheel, scratch cards, idle/tycoon builders, mining clickers — most of them live as Telegram Mini Apps, owning client and backend both:

- **Real-time multiplayer Texas Hold'em** — full poker engine with hand evaluation, ELO ranking tiers, a Spine-animated dealer, and bot AI running Monte-Carlo equity estimation, pot-odds analysis, and per-opponent behavioral modeling.
- **Authoritative game servers** on Colyseus + WebSockets, scaled horizontally with Redis presence/drivers, serving multiple concurrent rooms per process — live in production behind nginx with SSL, uptime monitoring, and Telegram ops alerts.
- **Casino & economy math done properly** — cryptographically seeded weighted RNG (`crypto.randomInt`, never `Math.random`), payout distribution, staking economies, `decimal.js` money handling.
- **Blockchain across three ecosystems** — **Bitcoin** (BIP32/39/86/322 HD derivation for per-user deposit addresses, withdrawal signing, Ordinals/Runes), **TON** (payments, wallet connect, Telegram Stars), **EVM** (Solidity/Hardhat, including commit-reveal and **ZK-SNARK (Circom)** versions of an on-chain game).
- **Hand-written GLSL shaders**, Spine skeletal animation, procedural effects, and a reusable responsive UI framework shared across every client.

## 📓 How I work

Substantial work lands in a plain-Markdown documentation vault — architecture notes, decision records, runbooks, and a dated worklog recording what changed and the **verified** outcome, including what was left undone. Docs ship in the same commit as the code: a stale README is a bug.

## 🛠 Stack

**Game clients**

![Cocos Creator](https://img.shields.io/badge/Cocos_Creator-55C2E1?style=flat-square&logo=cocos&logoColor=white)
![Phaser](https://img.shields.io/badge/Phaser_3-8E44AD?style=flat-square)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![GLSL](https://img.shields.io/badge/GLSL-5586A4?style=flat-square&logo=opengl&logoColor=white)
![Spine](https://img.shields.io/badge/Spine_2D-FF4000?style=flat-square)

**Servers & realtime**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Colyseus](https://img.shields.io/badge/Colyseus-8E44AD?style=flat-square)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![WebSocket](https://img.shields.io/badge/WebSockets-2C3E50?style=flat-square)

**Data**

![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square)
![Chroma](https://img.shields.io/badge/Chroma-FFA800?style=flat-square)
![pgvector](https://img.shields.io/badge/pgvector-336791?style=flat-square)

**AI / LLM**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Anthropic](https://img.shields.io/badge/Anthropic-191919?style=flat-square&logo=anthropic&logoColor=white)
![RAG](https://img.shields.io/badge/RAG-6C3EB8?style=flat-square)
![Tool Calling](https://img.shields.io/badge/Tool_Calling-0A7E8C?style=flat-square)
![MCP](https://img.shields.io/badge/MCP-F97316?style=flat-square)
![Evals & Guardrails](https://img.shields.io/badge/Evals_%26_Guardrails-2D6A4F?style=flat-square)
![Hugging Face](https://img.shields.io/badge/Transformers.js-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

**Web**

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-2C2C2C?style=flat-square)
![Framer Motion](https://img.shields.io/badge/Framer_Motion-0055FF?style=flat-square&logo=framer&logoColor=white)

**Blockchain**

![Bitcoin](https://img.shields.io/badge/Bitcoin-F7931A?style=flat-square&logo=bitcoin&logoColor=white)
![Arch Network](https://img.shields.io/badge/Arch_Network-E8622C?style=flat-square)
![BIP-322](https://img.shields.io/badge/BIP--322_Signing-4A4A4A?style=flat-square)
![TON](https://img.shields.io/badge/TON-0098EA?style=flat-square&logo=ton&logoColor=white)
![Ethereum](https://img.shields.io/badge/Ethereum-3C3C3D?style=flat-square&logo=ethereum&logoColor=white)
![Solidity](https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white)
![Circom](https://img.shields.io/badge/ZK--SNARKs_·_Circom-1A1A2E?style=flat-square)
![Telegram](https://img.shields.io/badge/Telegram_Mini_Apps-26A5E4?style=flat-square&logo=telegram&logoColor=white)

**Ops**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![nginx](https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![PM2](https://img.shields.io/badge/PM2-2B037A?style=flat-square&logo=pm2&logoColor=white)
![systemd](https://img.shields.io/badge/systemd-30D475?style=flat-square&logo=systemd&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![AWS](https://img.shields.io/badge/AWS_S3-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)

## 📍 Currently

- Taking **Archade** to production on Arch Network — a real-money cutover, so it moves at the pace the audit trail justifies
- Working through a structured AI-engineering roadmap, currently on **evals, guardrails, and LLM-app reliability**
- Open to interesting problems in **game backends, real-time systems, and applied AI**

---

<div align="center">

🌐 **[pyrotheum1702.com](https://pyrotheum1702.com/)** — my portfolio, with PyroBot on board if you'd rather ask it about me

</div>
