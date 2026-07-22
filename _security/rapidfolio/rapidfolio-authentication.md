---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Rapidfolio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rapidfolio secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rapidfolio
provider_slug: rapidfolio
scheme_count: 2
schemes:
- description: The Rapidfolio Runner API and Dashboard API authenticate with API keys. Keys are scoped per environment (separate sandbox and live keys) and are created, listed, and deleted via the Dashboard API. Documented in the "Authentication" and "API Keys" sections of the API reference.
  docs: https://docs.rapidfolio.com/docs/api/authentication
  in: header
  name: apiKey
  type: apiKey
- description: Private Connections (Node.js Connection SDK) authenticate with a per environment long-lived token supplied via the RAPID_TOKEN environment variable. Token format run_sandbox_… (Sandbox) or run_live_… (Live); rotate with "Regenerate token" in the dashboard.
  docs: https://docs.rapidfolio.com/docs/sdk/connection-sdk
  in: token
  name: connection-token
  type: apiKey
slug: rapidfolio-authentication
source_filename: rapidfolio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.rapidfolio.com/llms.txt\ndocs: https://docs.rapidfolio.com/docs/api/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  environments: [sandbox, live]\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    description: >-\n      The Rapidfolio Runner API and Dashboard API authenticate with API keys.\n      Keys are scoped per environment (separate sandbox and live keys) and are\n      created, listed, and deleted via the Dashboard API. Documented in the\n      \"Authentication\" and \"API Keys\" sections of the API reference.\n    docs: https://docs.rapidfolio.com/docs/api/authentication\n  - name: connection-token\n    type: apiKey\n    in: token\n    description: >-\n      Private Connections (Node.js Connection SDK) authenticate with a per\n      environment long-lived token supplied via the RAPID_TOKEN environment\n      variable. Token format run_sandbox_… (Sandbox) or run_live_…\
  \ (Live);\n      rotate with \"Regenerate token\" in the dashboard.\n    docs: https://docs.rapidfolio.com/docs/sdk/connection-sdk\nnotes: >-\n  No public OpenAPI/Swagger specification is published (the developer docs are\n  gated behind WorkOS AuthKit), so this profile is searched from the public\n  llms.txt index and the public @rapidfolio/connection-sdk-node README rather\n  than derived from a spec. Rapidfolio's own API is API-key based; OAuth appears\n  only in third-party Connections (Slack, Stripe, Xero, etc.), not on the\n  Rapidfolio API itself.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidfolio/refs/heads/main/authentication/rapidfolio-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Financial Services
- Fintech
- Workflow Automation
- Artificial Intelligence
- Agents
- Compliance
- KYC
- Fraud
- Back Office
---
