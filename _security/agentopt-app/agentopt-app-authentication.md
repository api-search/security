---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http-bearer
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Agentopt App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Priorflow secures its APIs with apiKey and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Priorflow
provider_slug: agentopt-app
scheme_count: 2
schemes:
- description: Paid-tier API key. Free tier works without a key (limited fields). Invalid keys are rejected. (verbatim from the agent card securitySchemes.apiKey.description)
  in: header
  issuance:
    checkout_body_example: '{"customer_email":"sponsor@example.com","client_reference_id":"tenant-1"}'
    checkout_operation: POST https://agentopt.app/v1/billing/checkout
    docs: https://agentopt.app/upgrade
    human_return_url: https://agentopt.app/upgrade/success?session_id=…
    mode: checkout
    operator_issued: Operators can still mint keys with create_api_key.py. (verbatim, /upgrade)
    reveal_operation: GET https://agentopt.app/v1/billing/session/{session_id}/key (one-time)
    summary: POST /v1/billing/checkout then reveal key once via GET /v1/billing/session/{session_id}/key; agents use X-API-Key thereafter. (verbatim, agent card priorflow.upgrade.obtain.summary)
  key_prefix: pf_live_
  key_prefix_evidence: 'The /upgrade page example reads X-API-Key: pf_live_… and the /try page labels its operator-published evaluation key with the same prefix.'
  name: apiKey
  parameter: X-API-Key
  sources:
  - a2a/agentopt-app-agent-card.json
  - https://agentopt.app/upgrade
  type: apiKey
  used_by:
  - 'POST /v1/select (paid tier: unlocks tags, dimensions, score_breakdown, recommendation, clarifications, source_url, endpoint/connect, homepage_url, endpoint_status; top_n up to 20; include_explanations)'
- description: 'Also accepted: Authorization: Bearer …. Invalid keys always return 401. (verbatim, /upgrade "How agents use paid access")'
  name: bearer
  note: The same pf_live_ key carried as a bearer token instead of X-API-Key. Declared only in the card's legacy authentication block (schemes [Bearer, ApiKey]) and on the /upgrade page, not in securitySchemes.
  scheme: bearer
  sources:
  - a2a/agentopt-app-agent-card.json
  - https://agentopt.app/upgrade
  type: http
slug: agentopt-app-authentication
source_filename: agentopt-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://agentopt.app/.well-known/agent-card.json\ndocs:\n- https://agentopt.app/info\n- https://agentopt.app/upgrade\nsummary:\n  types:\n  - apiKey\n  - http-bearer\n  api_key_in:\n  - header\n  oauth2_flows: []\n  bearer: true\n  credential_classes: 2\n  headline: >-\n    Two tiers, one credential. The free tier needs no credential at all — only a non-empty User-Agent header\n    and, by convention, a stable caller_agent string in the body — and is open on this host while\n    require_api_key is false (confirmed live via GET /ready). The paid tier uses a key sent as X-API-Key,\n    or equivalently as Authorization: Bearer; keys are issued to a human \"sponsor\" once (Stripe Checkout at\n    POST /v1/billing/checkout, one-time reveal at GET /v1/billing/session/{session_id}/key, or minted by the\n    operator) and agents use them autonomously thereafter. Invalid keys always return 401; paid-only\n    features without a key\
  \ return 402 upgrade_required. No OAuth, no OIDC, no discovery documents.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Paid-tier API key. Free tier works without a key (limited fields). Invalid keys are rejected. (verbatim from the agent card securitySchemes.apiKey.description)'\n  key_prefix: pf_live_\n  key_prefix_evidence: 'The /upgrade page example reads X-API-Key: pf_live_… and the /try page labels its operator-published evaluation key with the same prefix.'\n  issuance:\n    mode: checkout\n    summary: 'POST /v1/billing/checkout then reveal key once via GET /v1/billing/session/{session_id}/key; agents use X-API-Key thereafter. (verbatim, agent card priorflow.upgrade.obtain.summary)'\n    checkout_operation: POST https://agentopt.app/v1/billing/checkout\n    checkout_body_example: '{\"customer_email\":\"sponsor@example.com\",\"client_reference_id\":\"tenant-1\"}'\n    reveal_operation: 'GET https://agentopt.app/v1/billing/session/{session_id}/key\
  \ (one-time)'\n    human_return_url: 'https://agentopt.app/upgrade/success?session_id=…'\n    operator_issued: 'Operators can still mint keys with create_api_key.py. (verbatim, /upgrade)'\n    docs: https://agentopt.app/upgrade\n  used_by: ['POST /v1/select (paid tier: unlocks tags, dimensions, score_breakdown, recommendation, clarifications, source_url, endpoint/connect, homepage_url, endpoint_status; top_n up to 20; include_explanations)']\n  sources:\n  - a2a/agentopt-app-agent-card.json\n  - https://agentopt.app/upgrade\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'Also accepted: Authorization: Bearer …. Invalid keys always return 401. (verbatim, /upgrade \"How agents use paid access\")'\n  note: The same pf_live_ key carried as a bearer token instead of X-API-Key. Declared only in the card's legacy authentication block (schemes [Bearer, ApiKey]) and on the /upgrade page, not in securitySchemes.\n  sources:\n  - a2a/agentopt-app-agent-card.json\n  - https://agentopt.app/upgrade\n\
  anonymous_access:\n  allowed: true\n  evidence: 'agent card security: [] and priorflow.api.select.require_api_key false; /ready require_api_key false (fetched 2026-09-19)'\n  conditions:\n  - 'Requires non-empty User-Agent on free calls. (card, select-agents skill)'\n  - 'Always send a non-empty User-Agent and a stable caller_agent. (/info, Integrate)'\n  - 'Free tier returns id, score, score_band, name only; top_n <= 5; lower RPM (roughly 20/min, 120/hour, 500/day per IP).'\n  - 'The operator can close the free tier: \"free tier open on this host when enabled\".'\nfailure_semantics:\n  invalid_key: 401 (always)\n  paid_feature_without_key: 402 upgrade_required (when enabled)\n  exhausted_pack: 402 select_quota_exceeded or api_key_expired\n  detail: errors/agentopt-app-problem-types.yml\nnot_present:\n  oauth2: false\n  oidc: false\n  mutual_tls: false\n  discovery_documents: '/.well-known/oauth-authorization-server and /.well-known/openid-configuration both 404 (well-known/agentopt-app-well-known.yml)'\n\
  note: >-\n  No OpenAPI exists to derive from, so derive-authentication.py had nothing to read; this profile is\n  searched from the agent card's securitySchemes and the /info and /upgrade pages. The evaluation key the\n  operator publishes on /try is deliberately NOT recorded here or anywhere in this repo — it is a live paid\n  credential drawn from a shared, expiring quota pool, not a test-mode value (see sandbox/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentopt-app/refs/heads/main/authentication/agentopt-app-authentication.yml
summary_line: apiKey/http-bearer · 2 schemes
tags:
- AI Agents
- Agent Discovery
- Agent Selection
- A2A
- MCP
- Agent Orchestration
- Tool Ranking
- Semantic Search
- agent-native
---
