---
anonymous_access: true
api_key_in: []
api_specs:
- filename: opplevagent-no-openapi.yml
  format: yaml
  label: Opplevagent Discovery API
  slug: discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opplevagent-no/refs/heads/main/openapi/opplevagent-no-openapi.yml
auth_types:
- none
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Opplevagent No Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opplevagent secures its APIs with none and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Opplevagent
provider_slug: opplevagent-no
scheme_count: 2
schemes:
- description: Default. Every documented operation, MCP tool and A2A skill accepts unauthenticated calls.
  name: anonymous
  sources:
  - openapi/opplevagent-no-openapi.yml (info.description)
  - https://opplevagent.no/.well-known/mcp/server-card.json (authentication.schemes [none])
  - https://opplevagent.no/.well-known/agent-card.json (authentication.schemes [none])
  type: none
- description: Voluntary, free identity key for AI agents. No login, account or identity check — issued instantly by POST /api/keys. Sending it raises the rate ceiling roughly 3x (200 -> 600 per 900 s on /a2a and /mcp, 300 -> 900 on REST) and records calls in an aggregated per-key usage ledger (endpoint/tool name and date only, never content or arguments).
  header: X-API-Key
  in: header
  name: consumerApiKey
  required: false
  sources:
  - https://opplevagent.no/llms.txt ("Frivillig API-nøkkel (forbruker-identitet)")
  - https://opplevagent.no/.well-known/agent-card.json (securitySchemes.consumerApiKey)
  type: apiKey
slug: opplevagent-no-authentication
source_filename: opplevagent-no-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://opplevagent.no/llms.txt\ndocs: https://opplevagent.no/llms.txt\nspec: openapi/opplevagent-no-openapi.yml\nsummary:\n  types:\n  - none\n  - apiKey\n  required: false\n  transport: X-API-Key request header, HTTPS only\n  note: >-\n    The OpenAPI declares no securitySchemes and no security requirement, and states \"All read endpoints are public;\n    no authentication required.\" The provider's llms.txt, agent card (securitySchemes.consumerApiKey) and MCP server\n    card all say the same: every REST, MCP and A2A call works anonymously. An optional, free consumer key exists\n    purely as an identity/rate-tier signal. derive-authentication.py produced no profile because the spec is\n    scheme-less; this file records the documented model instead.\nschemes:\n- name: anonymous\n  type: none\n  description: Default. Every documented operation, MCP tool and A2A skill accepts unauthenticated calls.\n  sources:\n  - openapi/opplevagent-no-openapi.yml\
  \ (info.description)\n  - https://opplevagent.no/.well-known/mcp/server-card.json (authentication.schemes [none])\n  - https://opplevagent.no/.well-known/agent-card.json (authentication.schemes [none])\n- name: consumerApiKey\n  type: apiKey\n  in: header\n  header: X-API-Key\n  required: false\n  description: >-\n    Voluntary, free identity key for AI agents. No login, account or identity check — issued instantly by POST\n    /api/keys. Sending it raises the rate ceiling roughly 3x (200 -> 600 per 900 s on /a2a and /mcp, 300 -> 900 on\n    REST) and records calls in an aggregated per-key usage ledger (endpoint/tool name and date only, never content\n    or arguments).\n  sources:\n  - https://opplevagent.no/llms.txt (\"Frivillig API-nøkkel (forbruker-identitet)\")\n  - https://opplevagent.no/.well-known/agent-card.json (securitySchemes.consumerApiKey)\ncredentials:\n- id: consumer-key\n  header: 'X-API-Key: <key>'\n  prefix: null\n  use: Optional higher rate-limit tier on any REST, MCP\
  \ or A2A call\n  issued_by: >-\n    POST https://opplevagent.no/api/keys — optional JSON body {\"label\": \"...\", \"contact_email\": \"...\"}; the\n    response contains `key`, shown once and not retrievable again\n  lifecycle:\n    revoke: POST https://opplevagent.no/api/keys/revoke — stops the key, retains history\n    erase: POST https://opplevagent.no/api/keys/erase — GDPR deletion of label and e-mail\n    body: '{\"key\": \"...\"} or the key as the X-API-Key header'\n  note: >-\n    The key lifecycle endpoints are documented in llms.txt but are not declared in the OpenAPI (see\n    overlays/opplevagent-no-api-overlay.yaml). The agent card warns that the same header name may elsewhere denote\n    a producer/write key, but opplevagent.no has no write API behind it, so here X-API-Key means only this key.\noauth: null\nscopes: null\nmcp_auth:\n  scheme: none\n  session: mcp-session-id header issued on initialize and required on every later call (a transport session, not a credential)\n\
  a2a_auth:\n  scheme: none\n  card_declares: authentication.schemes [none]; securitySchemes.consumerApiKey optional\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opplevagent-no/refs/heads/main/authentication/opplevagent-no-authentication.yml
summary_line: none/apiKey · 2 schemes
tags:
- Travel
- Tourism
- Experience
- Activities
- Norway
- Marketplace
- agent-native
- A2A
- MCP
- Booking
- Local Food
- Open Data
---
