---
api_key_in:
- query
- body
auth_types:
- apiKey
- wallet
description: ''
kind: authentication
layout: security
method: searched
name: My Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: My AI secures its APIs with apiKey and wallet across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: My AI
provider_slug: my-ai
scheme_count: 2
schemes:
- description: Brand/merchant API key issued by Me Protocol, passed by the PaaS SDKs (payWithMePaas, MeAgent) to authenticate reward and payment calls against the hosted PaaS API (paas.memarketplace.io/v1/api). Each environment (dev/staging/prod) carries its own key.
  in: query
  name: PaaS API Key
  parameter: apiKey
  sources:
  - packages/my-ai-packages.yml
  type: apiKey
- description: End-user authentication via Magic (magic.link) publishable key for email-based wallet creation, used to authorize on-chain reward redemption and cross-brand token swaps. Networks — Sepolia, Hedera, Base, Polygon.
  name: Magic Link Wallet Auth
  scheme: magic-link
  sources:
  - packages/my-ai-packages.yml
  type: wallet
slug: my-ai-authentication
source_filename: my-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/Me-Protocol/me-agent-sdk (SDK config) + https://me-api-docs.pages.dev/\ndocs: https://me-api-docs.pages.dev/\nsummary:\n  types:\n  - apiKey\n  - wallet\n  api_key_in:\n  - query\n  - body\nnote: No public OpenAPI is published; this profile is derived from the first-party\n  SDK source and hosted PaaS API behavior rather than a machine-readable securityScheme.\nschemes:\n- name: PaaS API Key\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: Brand/merchant API key issued by Me Protocol, passed by the PaaS SDKs\n    (payWithMePaas, MeAgent) to authenticate reward and payment calls against the\n    hosted PaaS API (paas.memarketplace.io/v1/api). Each environment (dev/staging/prod)\n    carries its own key.\n  sources:\n  - packages/my-ai-packages.yml\n- name: Magic Link Wallet Auth\n  type: wallet\n  scheme: magic-link\n  description: End-user authentication via Magic (magic.link) publishable\
  \ key for\n    email-based wallet creation, used to authorize on-chain reward redemption and\n    cross-brand token swaps. Networks — Sepolia, Hedera, Base, Polygon.\n  sources:\n  - packages/my-ai-packages.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/my-ai/refs/heads/main/authentication/my-ai-authentication.yml
summary_line: apiKey/wallet · 2 schemes
tags:
- Company
- Rewards
- Loyalty
- Web3
- Blockchain
- API
- SDK
- AI Agent
- Payments
- Smart Contracts
---
