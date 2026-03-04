# Digital Money Center (DMC) Core Ecosystem

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)]()
[![Network: Base](https://img.shields.io/badge/Network-Base-blue.svg)]()

**Wyoming's Regulated Fintech Money Center for the Underserved.**

Digital Money Center (DMC) is a unified fintech application bridging traditional finance, physical commodities, and digital assets. Operating as a Wyoming DAO LLC under Money Transmitter and Consumer Lender licenses, DMC provides instant liquidity and AI-underwritten capital to unbanked demographics, rural infrastructure projects, and impact-driven entrepreneurs.

## Core Capabilities

* **Instant Liquidity:** Digital check cashing and rapid micro-loans.
* **Physical Commodities:** Direct purchase and vaulting of physical gold and silver (via Constitutional Tender, LLC integration).
* **Digital Assets:** Crypto on/off-ramps (BTC, ETH, SOL, Stablecoins).
* **Global Remittances:** Real-time FX transfers powered by JP Morgan Payments.
* **Impact Finance:** CDFI-aligned capital pools for agricultural and biomass energy projects (e.g., Ryegate facility fertilizer loops).

## The $DMC Utility Token

The ecosystem is powered by **$DMC**, a pure consumptive-use ERC-20 utility token deployed on the Base network. 

* **Fee Reduction:** Paying network fees in $DMC unlocks automated 30–50% discounts.
* **Deflationary Mechanics:** Every transaction fee paid in $DMC triggers an automatic burn.
* **Governance:** Token staking grants voting rights within the Wyoming DAO LLC structure and priority access to the AI underwriting queue.

## System Architecture

DMC utilizes a modern, compliance-first technology stack:

* **Frontend / Core Banking UI:** Next.js 15, Tailwind CSS, Nymbus Connect SDK.
* **Backend:** NestJS, Prisma, PostgreSQL.
* **Intelligence Layer:** NVIDIA Triton Inference Server running XGBoost/LightGBM ensembles. Full SHAP explainability is logged for regulatory compliance and fair-lending audits.
* **Blockchain & Oracles:** Hardhat/Foundry, deployed on Base. Real-time asset pricing via Chainlink and Pyth network oracles.
* **Infrastructure:** Terraform, AWS GovCloud (for PII and financial records).

## Repository Structure

```text
dmc-core/
├── apps/
│   ├── web/                # Next.js web application
│   ├── mobile/             # React Native mobile application
│   └── admin-dashboard/    # Internal CDFI & AML reporting tools
├── packages/
│   ├── contracts/          # ERC-20 $DMC Token, Staking, and Governance (Solidity)
│   ├── ai-engine/          # Python 3.12 models, SHAP explainers, Triton configs
│   └── shared-types/       # TypeScript interfaces used across the monorepo
├── infrastructure/         # Terraform configurations for AWS and Node deployments
├── docs/                   # Whitepaper, Developer Handbook, and SOW
└── .github/                # CI/CD workflows and security scanning parameters
