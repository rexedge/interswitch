# Interswitch Skills Collection

> **18 modular AI agent skills for [Interswitch](https://www.interswitchgroup.com/) payment integration** — TypeScript, Node.js, and Next.js ready.

Build payment systems, wallets, card processing, transfers, VAS, and more with production-ready Interswitch API patterns. Each skill teaches your AI coding agent exactly how to integrate a specific part of the Interswitch API — type-safe, tested, and ready to ship.

[![Skills](https://img.shields.io/badge/skills.sh-18_skills-blue)](https://skills.sh)
[![Interswitch](https://img.shields.io/badge/Interswitch-API-green)](https://www.interswitchgroup.com/)
[![TypeScript](https://img.shields.io/badge/TypeScript-Ready-3178C6)](https://www.typescriptlang.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## Why Use Interswitch Skills?

- **Modular** — Install only the skills you need, not a monolithic guide
- **Type-safe** — Full TypeScript support with Zod validation and typed responses
- **Production-ready** — Battle-tested patterns with error handling and security
- **AI-powered** — Designed for AI coding agents (GitHub Copilot, Cursor, etc.)
- **Comprehensive** — 18 skills covering Interswitch's payment, wallet, card, transfer, and VAS APIs

## Quick Start

```bash
# Install all 18 skills at once
npx skills add rexedge/interswitch --all

# Install a specific skill
npx skills add rexedge/interswitch -s interswitch-web-checkout

# Install multiple specific skills
npx skills add rexedge/interswitch -s interswitch-setup interswitch-webhooks interswitch-card-payments
```

## Available Skills

### Core

| Skill | Description |
| --- | --- |
| [interswitch-setup](skills/interswitch-setup/) | API client setup, OAuth 2.0 token generation, Passport v2 auth, env config, TypeScript helpers |
| [interswitch-webhooks](skills/interswitch-webhooks/) | HmacSHA512 signature validation, event handling, Express.js & Next.js handlers, retry policy |
| [interswitch-testing](skills/interswitch-testing/) | Test credentials, test card numbers, sandbox URLs, webhook testing, going-live checklist |

### Payments & Checkout

| Skill | Description |
| --- | --- |
| [interswitch-web-checkout](skills/interswitch-web-checkout/) | Inline Checkout JS widget, Web Redirect HTML form, React/Next.js hook, redirect callback |
| [interswitch-card-payments](skills/interswitch-card-payments/) | Direct card payment, authData encryption, OTP validation, 3D Secure, Hosted Fields, Google Pay |
| [interswitch-payment-links](skills/interswitch-payment-links/) | Create, list, update, deactivate payment links — invoices, donations, tickets |
| [interswitch-split-settlement](skills/interswitch-split-settlement/) | Split payments, beneficiary configuration, wallet-pay initialization, settlement accounts |

### Wallets & Transactions

| Skill | Description |
| --- | --- |
| [interswitch-wallets](skills/interswitch-wallets/) | Create wallet, get details, check balance, virtual cards, Zod validation |
| [interswitch-transactions](skills/interswitch-transactions/) | Debit wallet, transaction status, requery, reversal, response codes |
| [interswitch-transaction-search](skills/interswitch-transaction-search/) | Quick search, reference search, advanced/bulk search, reconciliation pattern |

### Transfers & Payouts

| Skill | Description |
| --- | --- |
| [interswitch-transfers](skills/interswitch-transfers/) | Account validation (name enquiry), MAC hash (SHA-512), single transfer, status check |
| [interswitch-payouts](skills/interswitch-payouts/) | Payout channels, receiving institutions, institution details, routing logic |

### Value Added Services

| Skill | Description |
| --- | --- |
| [interswitch-vas](skills/interswitch-vas/) | Biller categories, payment items, customer validation, bill payment, airtime recharge |

### Cards & Fintech

| Skill | Description |
| --- | --- |
| [interswitch-card360](skills/interswitch-card360/) | Card issuance (virtual/physical), PIN management, block/unblock, balance inquiry |
| [interswitch-fintech-cards](skills/interswitch-fintech-cards/) | Card debit, reversal, balance enquiry, lien place/release |
| [interswitch-cardless](skills/interswitch-cardless/) | Single/bulk paycode generation, status check, cancellation, ATM withdrawal |

### Insights & Data

| Skill | Description |
| --- | --- |
| [interswitch-customer-insights](skills/interswitch-customer-insights/) | Demographics, financial history, financial habits, KYC flow, NDPR compliance |
| [interswitch-lending](skills/interswitch-lending/) | Nano loans, salary lending, value financing, eligibility check, repayment |

## Use Cases

These skills help your AI agent build:

- **E-commerce checkout** — Web Checkout + Card Payments + Webhooks
- **Wallet platform** — Wallets + Transactions + Transfers
- **Marketplace payments** — Split Settlement + Transfers + Payouts
- **Bill payment app** — VAS + Wallets + Transactions
- **Card management** — Card 360 + Fintech Cards + Cardless
- **Lending/credit** — Lending + Customer Insights + Wallets
- **Payout system** — Transfers + Payouts + Transaction Search

## Interswitch API Reference

| Property | Value |
| --- | --- |
| Base URL (Sandbox) | `https://qa.interswitchng.com` |
| Base URL (Production) | `https://saturn.interswitchng.com` |
| Auth | OAuth 2.0 Bearer Token or Passport v2 (InterswitchAuth) |
| Content Type | `application/json` |
| Amount Unit | Kobo (multiply naira × 100) |

## Quick Links

- [Interswitch API Documentation](https://docs.interswitchgroup.com/docs/home)
- [Interswitch Developer Portal](https://developer.interswitchgroup.com/)
- [Skills Registry](https://skills.sh)
- [Report an Issue](https://github.com/rexedge/interswitch/issues)
- [Discussions](https://github.com/rexedge/interswitch/discussions)

## Contributing

Found an issue or want to improve a skill? [Open an issue](https://github.com/rexedge/interswitch/issues) or submit a pull request.

## License

MIT
