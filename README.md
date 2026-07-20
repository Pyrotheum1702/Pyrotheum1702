# Hi, I'm Nguyễn Quang Được (Pyro) 👋

**Full-stack game developer** from Hà Nội, Việt Nam — I build real-time multiplayer web games end to end: the client, the authoritative server, the economy math, and the infrastructure they run on. Currently expanding into **AI engineering**, shipping production LLM applications along the way.

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

| Area             | Tools                                                               |
| ---------------- | ------------------------------------------------------------------- |
| **Game clients** | Cocos Creator, TypeScript, GLSL, Spine                              |
| **Servers**      | Node.js, Colyseus, Express, FastAPI (Python)                        |
| **Data**         | MongoDB, Redis, PostgreSQL, Chroma / Qdrant / pgvector              |
| **AI/LLM**       | LangChain, RAG, tool calling, streaming, embeddings, MCP            |
| **Web**          | React, Next.js, Vite, Tailwind, Framer Motion                       |
| **Blockchain**   | Bitcoin (bitcoinjs, BIP32/39/322), TON SDK, ethers/Solidity, Circom |
| **Ops**          | Docker, nginx, PM2, Prometheus, GitHub Actions, AWS S3              |

## 📍 Currently

- Taking a game to production on **Arch Network** (Bitcoin L2) with token integration
- Working through a structured AI-engineering roadmap: agents, evals, and LLM-app reliability
- Open to interesting problems in **game backends, real-time systems, and applied AI**

---

🌐 **[pyrotheum1702.com](https://pyrotheum1702.com/)** — my portfolio, with PyroBot on board if you'd rather ask it about me
📫 Reach me: **pyrotheum1702@gmail.com**