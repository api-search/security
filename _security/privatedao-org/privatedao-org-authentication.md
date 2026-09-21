---
anonymous_access: true
api_key_in: []
api_specs:
- filename: privatedao-org-agent-exchange-openapi.yml
  format: yaml
  label: PrivateDAO Agent Exchange API
  slug: agent-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-agent-exchange-openapi.yml
- filename: privatedao-org-blind-policy-openapi.yml
  format: yaml
  label: PrivateDAO Blind Policy Verification API
  slug: blind-policy-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-blind-policy-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Privatedao Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: PrivateDAO declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: PrivateDAO
provider_slug: privatedao-org
scheme_count: 2
schemes:
- apis:
  - agent-exchange
  - blind-policy
  evidence: Agent Card authentication.schemes includes "none"; every GET and the free createJob services were called anonymously during this pass.
  id: none
  type: none
- apis:
  - agent-exchange
  evidence: Agent Card authentication.schemes includes "solana-payment"; workflow.paid and payment blocks; llms.txt flow line.
  field: payment_intent
  flow: POST /api/jobs -> 402 payment_intent (exact USDC quote + treasury token account) -> agent signs its own finalized USDC transfer on solana:mainnet-beta -> POST /api/jobs/{jobId}/payment {signature} -> GET /api/jobs/{jobId}
  id: solana-payment
  note: Not a registered A2A/OpenAPI security scheme type; it authorises one job, not a caller.
  status_code: 402
  type: payment-gate
slug: privatedao-org-authentication
source_filename: privatedao-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://agents.privatedao.org/.well-known/agent-card.json (authentication.schemes), https://agents.privatedao.org/llms.txt,\n  both OpenAPIs (no components.securitySchemes, no security requirement), https://privatedao.org/developers/blind-policy-api/\n  and /blind-policy-sdk/ (client created with baseUrl only, no credential), CORS preflight headers observed on api.privatedao.org\n  (2026-09-19).\ndocs: https://agents.privatedao.org/llms.txt\nsummary: 'Neither public API requires a credential. The Agent Exchange gates paid services by payment, not identity:\n  a paid createJob returns 402 with a payment_intent and is unlocked by submitting a finalized Solana mainnet USDC\n  transaction signature. The Blind Policy API console and SDK call https://api.privatedao.org/api/v1 with no key.\n  derive-authentication.py found no securitySchemes in either spec, which is why this profile is hand-written from\n  the docs rather than derived.'\n\
  schemes:\n- id: none\n  type: none\n  apis:\n  - agent-exchange\n  - blind-policy\n  evidence: Agent Card authentication.schemes includes \"none\"; every GET and the free createJob services were called\n    anonymously during this pass.\n- id: solana-payment\n  type: payment-gate\n  apis:\n  - agent-exchange\n  status_code: 402\n  field: payment_intent\n  flow: POST /api/jobs -> 402 payment_intent (exact USDC quote + treasury token account) -> agent signs its own\n    finalized USDC transfer on solana:mainnet-beta -> POST /api/jobs/{jobId}/payment {signature} -> GET /api/jobs/{jobId}\n  evidence: Agent Card authentication.schemes includes \"solana-payment\"; workflow.paid and payment blocks; llms.txt\n    flow line.\n  note: Not a registered A2A/OpenAPI security scheme type; it authorises one job, not a caller.\nobserved_undocumented:\n- header: x-private-dao-operator-token\n  host: api.privatedao.org\n  evidence: Listed in access-control-allow-headers on https://api.privatedao.org/api/v1/proof-workflows/blind-policy/status\n\
  \  note: Not documented anywhere public; presumably guards operator/anchor routes outside the published Blind Policy\n    contract. Recorded as observed only - no route requiring it was identified and none was probed.\n- header: x-private-dao-anchor-token\n  host: api.privatedao.org\n  evidence: Same CORS allow-list\n  note: As above.\noauth2: null\nopenid_connect: null\napi_keys: null\nmutual_tls: null\ncross_links:\n  conventions: conventions/privatedao-org-conventions.yml\n  conformance: conformance/privatedao-org-conformance.yml\n  a2a: a2a/privatedao-org-a2a.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/authentication/privatedao-org-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Agents
- A2A
- MCP
- Verification
- Zero-Knowledge Proofs
- Solana
- Blockchain
- Payments
- Marketplace
- Privacy
- Governance
- Treasury
---
