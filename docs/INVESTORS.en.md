# CR404 NEXUS — investor note

English, short. The full argument is the [German README](../README.md).

![The cockpit](../media/nexus-cockpit.jpg)

**Automation that asks before it costs money.**

**CR404 NEXUS is an operating system for small, automatable businesses.**
Trading, commerce, a guardian, an app foundry and a studio share one cockpit.
Each piece is a product on its own. Together they are designed to land in one treasury.

This repository is a public dossier. It contains **no source code**.
The pictures are brand stills, not screenshots of the shipped UI.
Implementation stays in private working repositories and is shown in conversation, not by cloning this repo.

## See it

Both clips run in the cockpit's simulation mode. All figures are demo data and labelled as such on screen.

| Tante Emma: from find to approved listing | Dagobert Market: paper first, then approval |
| --- | --- |
| ![Tante Emma demo](../media/demo/tante-emma-desk-demo.gif) | ![Dagobert demo](../media/demo/dagobert-backtest-demo.gif) |

## The five

| Module | What it is | Sells alone | Honest status |
| --- | --- | --- | --- |
| **RoboCop404** | Guardian. Start, stop, audit, circuit breaker. | Yes, as an ops and security module | Cockpit plus a small rules-based security module. Deploys are drafts until a human approves. |
| **Tante Emma** | The shop. Retail plus B2B dropshipping. | Yes | UI and product model are in place. Marketplace publishers are skeletons, not a silent Amazon bot. |
| **Dagobert Market** | The desk. Signals, paper trade, backtests. Crypto first. | Yes | Dashboard runs. Live orders sit behind a gate. Not a broker, not a return. |
| **Forge** | The foundry. A sentence becomes a running app. | Yes | Pipeline really builds, boots the backend and commits locally. Remote push is off unless asked. |
| **Music Video Studio** | The studio. Prompt to track and picture. | Yes, once generation is wired | Architecture and a seat in the cockpit. Generators are the next build, not a finished button. |

Satellites, already cut as their own products: **AL Messenger** (realtime chat), **B2B arbitrage** (discovery, SEO, human approval before any public listing), **CR404 Shops** (storefronts the shop module can list from).

## Why the cut matters

A merchant can buy Tante Emma and ignore crypto.
A builder can buy Forge and ignore the shop.
The suite is the upsell, not the ticket in.

The thing worth underwriting is not "another agent".
It is a kit of markets, already split into repositories, with a human approval gate on the actions that can cost money or reputation: listings, deploys, live orders.

API keys are optional. The cockpit runs without them.
Keys unlock live prices, read-only exchange balances and model calls. They never belong in the browser.

## Where capital would work

1. Finish Tante Emma: one merchant, one marketplace, one listing a human has seen.
2. Keep Dagobert boring and compliant. Better data, explainable backtests, a locked live path. Not custody of client funds.
3. Make Forge repeatable: a theme per job, a delivery a customer can start without the author.
4. Studio: one path from prompt to file.
5. NEXUS itself: one tenant, a real ledger, separate customers. The cockpit today is local and honestly simulatable. The jump left is operations, not a new architecture.

Funding one module does not require funding the shell.
Funding the shell funds the glue and the ledger.

## Not this

This page is not a term sheet, not an offer of securities, not investment advice.
Trading can go to zero. Whether a module needs a license depends on the country and on whether other people's money moves.
As of this dossier, Dagobert is a decision and simulation cockpit with live trading locked.

GitHub: [@arondakoa](https://github.com/arondakoa)

© 2026 arondakoa (CR404). All rights reserved. No open-source license; text and data mining and AI training reserved. See [`LICENSE`](../LICENSE).
