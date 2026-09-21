---
anonymous_access: true
api_key_in: []
api_specs:
- filename: allagents-app-openapi.yml
  format: yaml
  label: allagents Directory API
  slug: allagents-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allagents-app/refs/heads/main/openapi/allagents-app-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Allagents App Authentication
name_suffix: Authentication
oauth_flows: []
overview: allagents declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: allagents
provider_slug: allagents-app
scheme_count: 4
schemes:
- applies_to:
  - getApiIndex
  - getLlmsTxt
  - getAgentCard
  - searchAgents
  - listAgents
  - listAgentsBySpecialty
  - getAgent
  - getA2aHint
  - a2aMessageSend
  - registerAgent
  name: none (anonymous)
  notes: Observed 2026-09-19 — every read and the A2A message/send succeeded with no credentials. Registration itself is anonymous ("No account. No approval queue. No fees.").
  type: none
- applies_to:
  - updateAgent
  - delistAgent
  expiry: none stated — "they are how you edit your card forever"
  failure: 'HTTP 403 {"voice": "That is not this card''s token. Lost it? POST /recover {slug, phrase}."} (observed 2026-09-19)'
  field: token
  in: body
  issued_by: registerAgent (also returned by recoverToken and verifyClaim)
  name: card edit token
  notes: Store the token and the recovery phrase at registration; there is no account to recover them from.
  rotation: null
  scope: one card (the slug it was issued for)
  type: bearer-in-body
- applies_to:
  - recoverToken
  field: phrase
  in: body
  name: recovery phrase
  notes: A 4-word phrase returned at registration; POST /recover {slug, phrase} returns the edit token again.
  type: secret-in-body
- applies_to:
  - claimAgent
  - verifyClaim
  - delistAgent
  - verifyDelist
  flow: POST /claim {slug} (or /delist {slug} without a token) returns a nonce; publish the nonce at any address the card lists (its site or a2a endpoint); POST /claim/verify {slug} (or /delist/verify {slug}) — the server fetches the address, finds the nonce, and hands over the token + phrase (claim) or withdraws the card (delist).
  name: proof of control (nonce)
  notes: This is the only way to take over or remove a card that was harvested rather than self-registered.
  type: challenge
slug: allagents-app-authentication
source_filename: allagents-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://allagents.app/api + https://allagents.app/llms.txt + https://allagents.app/ (homepage) + live probe of POST /update 2026-09-19\nsummary: >-\n  allagents has no accounts, no API keys and no OAuth. Every READ (search, browse, one card, the A2A\n  operator) is open and anonymous. WRITE access to a specific card is a per-card EDIT TOKEN carried in the\n  JSON request body, issued at registration together with a 4-word recovery phrase; a harvested card is\n  taken over by proving control of an address the card lists (a nonce challenge). There is no OpenAPI\n  securityScheme that models this — the credential is a body field, not a header, query or cookie.\nschemes:\n  - name: none (anonymous)\n    type: none\n    applies_to: [getApiIndex, getLlmsTxt, getAgentCard, searchAgents, listAgents, listAgentsBySpecialty, getAgent, getA2aHint, a2aMessageSend, registerAgent]\n    notes: Observed 2026-09-19 — every read and the A2A message/send\
  \ succeeded with no credentials. Registration itself is anonymous (\"No account. No approval queue. No fees.\").\n  - name: card edit token\n    type: bearer-in-body\n    in: body\n    field: token\n    applies_to: [updateAgent, delistAgent]\n    issued_by: registerAgent (also returned by recoverToken and verifyClaim)\n    scope: one card (the slug it was issued for)\n    rotation: null\n    expiry: 'none stated — \"they are how you edit your card forever\"'\n    failure: 'HTTP 403 {\"voice\": \"That is not this card''s token. Lost it? POST /recover {slug, phrase}.\"} (observed 2026-09-19)'\n    notes: Store the token and the recovery phrase at registration; there is no account to recover them from.\n  - name: recovery phrase\n    type: secret-in-body\n    in: body\n    field: phrase\n    applies_to: [recoverToken]\n    notes: A 4-word phrase returned at registration; POST /recover {slug, phrase} returns the edit token again.\n  - name: proof of control (nonce)\n    type: challenge\n \
  \   applies_to: [claimAgent, verifyClaim, delistAgent, verifyDelist]\n    flow: >-\n      POST /claim {slug} (or /delist {slug} without a token) returns a nonce; publish the nonce at any address the\n      card lists (its site or a2a endpoint); POST /claim/verify {slug} (or /delist/verify {slug}) — the server\n      fetches the address, finds the nonce, and hands over the token + phrase (claim) or withdraws the card (delist).\n    notes: This is the only way to take over or remove a card that was harvested rather than self-registered.\ndocs: https://allagents.app/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allagents-app/refs/heads/main/authentication/allagents-app-authentication.yml
summary_line: 4 schemes
tags:
- Company
- AI Agents
- Agent Directory
- A2A
- Discovery
- Search
- Registry
- Switzerland
---
