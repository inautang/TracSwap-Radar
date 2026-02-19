# TracSwap Radar 🔭⚡

> **P2P Swap Price Intelligence on the Intercom Agent Mesh**

A fork of [IntercomSwap](https://github.com/TracSystems/intercom-swap) that adds a real-time **swap radar dashboard** — live order book, price chart, agent feed, and a one-click non-custodial BTC ⚡ ↔ USDT (Solana) swap interface — all coordinated over Intercom P2P sidechannels.

---
<img width="1281" height="849" alt="image" src="https://github.com/user-attachments/assets/b22ba975-6f17-451d-9fee-7787b2988fdd" />

##  What Is TracSwap Radar?

TracSwap Radar lets you monitor and execute non-custodial cross-chain swaps in real time:

- **Live Order Book** — P2P RFQ bids & asks from Intercom maker agents
- **Price Chart** — VWAP from Intercom mesh, 1-minute candles
- **Agent Feed** — live messages from Intercom sidechain peers
- **Swap Widget** — initiate a BTC (Lightning) ↔ USDT (Solana SPL) atomic swap via HTLC in ~4 seconds
- **Market Stats** — 24h volume, active swaps, avg settlement time

All settlement is **non-custodial via HTLC**: BTC side over Lightning, USDT side on Solana. Quotes are negotiated over Intercom P2P sidechannels; best quote auto-selected.

---

##  How To Run

```bash
# 1. Clone this fork
git clone https://github.com/YOUR_USERNAME/intercom-swap
cd intercom-swap

# 2. Open the radar app
open app/index.html
# OR serve it:
npx serve app/
```

No build step needed — pure HTML/CSS/JS front-end. The swap logic hooks into the Intercom node via the standard sidechain API.

---

##  App Preview

![TracSwap Radar Screenshot](./screenshots/radar-ui.png)

The app features:
- Dark terminal aesthetic with scanline overlay
- Live-updating order book with depth visualization
- Price sparkline chart
- Agent mesh activity log
- One-click swap modal with HTLC progress

---

## 🛠 Skill File (for Agents)

See [`SKILL.md`](./SKILL.md) for agent instructions on how to interact with TracSwap Radar's RFQ API over Intercom sidechannels.

---

##  Trac Payout Address

> trac13l0xqxl6vsn7ep0j3zf5rr4w0etpvv2ms889w74fhjtcuq6ke68q3r0kj9

*(Replace with your actual Trac address to receive 500 TNK payout)*

---

##  Links

- Upstream Intercom: https://github.com/Trac-Systems/intercom
- IntercomSwap fork: https://github.com/TracSystems/intercom-swap
- Awesome Intercom list: https://github.com/Trac-Systems/awesome-intercom

---

## License

MIT — built on Trac Network / Intercom stack.
