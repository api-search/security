---
anonymous_access: true
api_key_in: []
auth_types:
- public-key-identity
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Digiant Nz Authentication
name_suffix: Authentication
oauth_flows: []
overview: digiantnz secures its APIs with public-key-identity across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: digiantnz
provider_slug: digiant-nz
scheme_count: 2
schemes:
- description: '"Supply your ed25519 public key on first request — becomes your agent_id and account key" (agent card identity block, pubkey_exchange: true). There is no signup, no API key issuance and no OAuth flow: the calling agent''s Ed25519 public key is its account identifier; the free tier is rate-limited per key and paid credit (satoshis over Lightning, when it opens) is presumably attached to the same key. The card does not state which header or JSON-RPC field carries the key or whether requests must be signed — that detail requires the (404) GitHub repository or a live paid session, neither of which was reachable.'
  name: Ed25519PublicKeyIdentity
  scheme: ed25519
  sources:
  - https://a2a-browser.digiant.nz/.well-known/agent.json
  type: public-key-identity
- description: GET /.well-known/agent.json, /health and /quote answer without any credential; POST / accepts an unauthenticated JSON-RPC envelope (unknown methods answer -32601).
  name: Anonymous
  sources:
  - https://a2a-browser.digiant.nz/robots.txt
  type: none
slug: digiant-nz-authentication
source_filename: digiant-nz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://a2a-browser.digiant.nz/.well-known/agent.json (identity block), https://a2a-browser.digiant.nz/quote, https://a2a-browser.digiant.nz/robots.txt; no OpenAPI exists to derive from\ndocs: null\nsummary:\n  types:\n  - public-key-identity\n  api_key_in: []\n  oauth2: false\n  openid_connect: false\n  signup_required: false\nschemes:\n- name: Ed25519PublicKeyIdentity\n  type: public-key-identity\n  scheme: ed25519\n  description: >-\n    \"Supply your ed25519 public key on first request — becomes your agent_id and account key\" (agent card identity block,\n    pubkey_exchange: true). There is no signup, no API key issuance and no OAuth flow: the calling agent's Ed25519 public key\n    is its account identifier; the free tier is rate-limited per key and paid credit (satoshis over Lightning, when it opens)\n    is presumably attached to the same key. The card does not state which header or JSON-RPC field carries the key or\n\
  \    whether requests must be signed — that detail requires the (404) GitHub repository or a live paid session, neither of\n    which was reachable.\n  sources:\n  - https://a2a-browser.digiant.nz/.well-known/agent.json\n- name: Anonymous\n  type: none\n  description: GET /.well-known/agent.json, /health and /quote answer without any credential; POST / accepts an unauthenticated JSON-RPC envelope (unknown methods answer -32601).\n  sources:\n  - https://a2a-browser.digiant.nz/robots.txt\ngaps:\n- header or field carrying the public key is undocumented\n- request signing / challenge-response is undocumented\n- payment binding between key and Lightning invoice is undocumented (paid tier not yet open)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digiant-nz/refs/heads/main/authentication/digiant-nz-authentication.yml
summary_line: public-key-identity · 2 schemes
tags:
- Company
- A2A
- Agents
- Web Search
- Web Scraping
- Search
- Micropayments
- Lightning
- New Zealand
---
