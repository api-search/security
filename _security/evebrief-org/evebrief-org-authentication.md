---
anonymous_access: false
api_key_in: []
api_specs:
- filename: evebrief-org-openapi.json
  format: json
  label: onchain-risk-oracle API
  slug: onchain-risk-oracle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evebrief-org/refs/heads/main/openapi/evebrief-org-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Evebrief Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: openclaw / evm-lab declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: openclaw / evm-lab
provider_slug: evebrief-org
scheme_count: 0
schemes: []
slug: evebrief-org-authentication
source_filename: evebrief-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/evebrief-org-openapi.json\ndocs:\n- https://oracle.evebrief.org/.well-known/agent-card.json\n- https://oracle.evebrief.org/.well-known/x402\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  bearer: false\n  credential_classes: 0\n  payment_gated: true\n  headline: >-\n    No credential of any kind. The OpenAPI declares no securitySchemes (derive-authentication.py found\n    nothing to derive), the agent card declares no securitySchemes or security, and no OAuth/OIDC discovery\n    document exists on either host. Access to the one functional operation (POST /) is gated by PAYMENT, not\n    identity: an unpaid call returns HTTP 402 with x402 v2 PaymentRequirements and the retry carries a\n    PAYMENT-SIGNATURE header proving settlement of 0.01 RLUSD on the XRP Ledger through the t54 facilitator.\n    The four GET routes (both card paths, the x402 manifest, /healthz) are free and anonymous.\nschemes: []\n\
  payment_gate:\n  name: x402\n  standard: x402 v2 (HTTP 402 payment challenge)\n  request_header: PAYMENT-SIGNATURE\n  challenge_header: PAYMENT-REQUIRED (base64 JSON PaymentRequirements; the same object is the 402 body)\n  observed: 'GET and POST https://oracle.evebrief.org/ without the header -> 402, body error \"PAYMENT-SIGNATURE header is required\", fresh invoiceId per challenge (2026-09-19)'\n  requirements:\n    scheme: exact\n    network: 'xrpl:0 (XRP Ledger mainnet)'\n    asset: RLUSD (hex 524C555344000000000000000000000000000000)\n    issuer: rMxCKbEDwqr76QuheSUMdEGf4B9xJ8m5De\n    amount: '0.01'\n    pay_to: rH2tcNh56xoLUssRubra7DSDCgrReSZodW\n    facilitator: https://xrpl-facilitator-mainnet.t54.ai\n    max_timeout_seconds: 600\n  applies_to: [jsonrpc__post]\n  free_operations: [agent_card__well_known_agent_json_get, agent_card_alt__well_known_agent_card_json_get, x402_manifest__well_known_x402_get, healthz_healthz_get]\n  sources:\n  - a2a/evebrief-org-agent-card.json (capabilities.extensions[0],\
  \ required true)\n  - well-known/evebrief-org-x402.json\n  - errors/evebrief-org-problem-types.yml (the observed 402)\n  note: >-\n    Recorded as a payment gate rather than an apiKey scheme on purpose: PAYMENT-SIGNATURE is not a static\n    credential a caller holds, it is a per-invoice proof of settlement, and modelling it as an API key would\n    tell an agent to go looking for a key that is never issued. No identity, no account, no scopes.\ndiscovery:\n- {url: 'https://oracle.evebrief.org/.well-known/oauth-authorization-server', status: 404}\n- {url: 'https://oracle.evebrief.org/.well-known/oauth-protected-resource', status: 404}\n- {url: 'https://oracle.evebrief.org/.well-known/openid-configuration', status: 404}\n- {url: 'https://evebrief.org/.well-known/oauth-authorization-server', status: 404}\n- {url: 'https://evebrief.org/.well-known/openid-configuration', status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evebrief-org/refs/heads/main/authentication/evebrief-org-authentication.yml
summary_line: 0 schemes
tags:
- Agents
- A2A
- x402
- XRPL
- Blockchain
- DeFi
- EVM
- Security
- Fraud Detection
- Risk Management
- Agent-Native
- Market Intelligence
---
