<div align="center">

# Hi, I'm Nguyễn Quang Được (Pyro) 👋

**Full-stack game developer · Hà Nội, Việt Nam**

*I build real-time multiplayer web games end to end — the client, the authoritative server,<br>the economy math, and the infrastructure they run on. Currently expanding into **AI engineering**.*

<a href="https://pyrotheum1702.com/"><img src="https://img.shields.io/badge/Portfolio-pyrotheum1702.com-FF6B35?style=for-the-badge&logo=firefoxbrowser&logoColor=white" alt="Portfolio"></a>
<a href="mailto:pyrotheum1702@gmail.com"><img src="https://img.shields.io/badge/Email-pyrotheum1702%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>

</div>

---

## 🎮 What I've Built

Over the past few years I've shipped **7+ game titles** — poker, slots, spin-wheel, scratch cards, idle/tycoon builders, and mining clickers — most of them live as Telegram Mini Apps, owning both client and backend:

- **Real-time multiplayer Texas Hold'em** — full poker engine with hand evaluation, ELO ranking tiers, Spine-animated dealer, and a bot AI that runs Monte-Carlo equity estimation, pot-odds analysis, and per-opponent behavioral modeling.
- **Authoritative game servers** on Colyseus + WebSockets, horizontally scaled with Redis presence/drivers, serving multiple concurrent game rooms per process — running live in production behind nginx with SSL, uptime monitoring, and Telegram ops alerts.
- **Casino & economy math done properly** — cryptographically seeded weighted RNG (`crypto.randomInt`, never `Math.random`), payout distribution, staking economies, and `decimal.js` money handling.
- **Blockchain integration across three ecosystems**:
  - **Bitcoin** — HD wallet derivation (BIP32/39/322) for per-user deposit addresses, withdrawal signing, Ordinals/Runes support
  - **TON** — payments, wallet connect, and Telegram Stars monetization inside Mini Apps
  - **EVM** — Solidity contracts (Hardhat), including a commit-reveal and **ZK-SNARK (Circom)** version of an on-chain game
- **Hand-written GLSL shaders**, Spine skeletal animation, procedural effects, and a reusable responsive UI framework shared across all my game clients.

## 🤖 AI Engineering

I'm documenting this journey publicly in [learning-ai-engineering](https://github.com/Pyrotheum1702/learning-ai-engineering) — code hand-written, AI used as a tutor.

- **[PyroBot](https://github.com/Pyrotheum1702/pyro-chat-bot)** — an agentic-RAG assistant embedded on my portfolio site. FastAPI + LangChain + Chroma + Fireworks, with a hand-written streaming tool-calling loop (SSE), four production tools, prompt-injection defenses, SSRF/path-traversal guards, rate limiting, and a daily LLM cost-cap kill-switch. Dockerized and deployed.
- **RAG in production games** — built an in-game AI guide with a Qdrant-backed retrieval pipeline, provider-agnostic LLM client, and function calling.
- **Agentic systems for clients** — FastAPI services orchestrating agent runtimes over MCP, with pgvector retrieval, deterministic validation gates, and human-approval workflows.

## 🛠 Stack

**Game clients**

![Cocos Creator](https://img.shields.io/badge/Cocos_Creator-55C2E1?style=flat-square&logo=cocos&logoColor=white)
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
![Hugging Face](https://img.shields.io/badge/Transformers.js-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

**Web**

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Framer Motion](https://img.shields.io/badge/Framer_Motion-0055FF?style=flat-square&logo=framer&logoColor=white)

**Blockchain**

![Bitcoin](https://img.shields.io/badge/Bitcoin-F7931A?style=flat-square&logo=bitcoin&logoColor=white)
![TON](https://img.shields.io/badge/TON-0098EA?style=flat-square&logo=ton&logoColor=white)
![Ethereum](https://img.shields.io/badge/Ethereum-3C3C3D?style=flat-square&logo=ethereum&logoColor=white)
![Solidity](https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white)
![Circom](https://img.shields.io/badge/ZK--SNARKs_·_Circom-1A1A2E?style=flat-square)
![Telegram](https://img.shields.io/badge/Telegram_Mini_Apps-26A5E4?style=flat-square&logo=telegram&logoColor=white)

**Ops**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![nginx](https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![PM2](https://img.shields.io/badge/PM2-2B037A?style=flat-square&logo=pm2&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![AWS](https://img.shields.io/badge/AWS_S3-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)

## 📍 Currently

- Taking a game to production on **Arch Network** (Bitcoin L2) with token integration
- Working through a structured AI-engineering roadmap: agents, evals, and LLM-app reliability
- Open to interesting problems in **game backends, real-time systems, and applied AI**

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Pyrotheum1702&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github" alt="GitHub stats" height="165">
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Pyrotheum1702&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top languages" height="165">

</div>

---

<div align="center">

🌐 **[pyrotheum1702.com](https://pyrotheum1702.com/)** — my portfolio, with PyroBot on board if you'd rather ask it about me
📫 **pyrotheum1702@gmail.com**

</div>
