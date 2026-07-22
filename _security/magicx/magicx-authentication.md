---
api_key_in: []
auth_types:
- http
description: AI Autocomplete authenticates every request to https://api.ai-autocomplete.com with an HTTP Bearer token. Three credential types are issued, all created from the account keys page (https://ai-autocomplete.com/account/keys).
kind: authentication
layout: security
method: searched
name: Magicx Authentication
name_suffix: Authentication
oauth_flows: []
overview: MagicX secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MagicX
provider_slug: magicx
scheme_count: 3
schemes:
- name: publicKey
  prefix: pk_v1_
  scheme: bearer
  source: https://ai-autocomplete.com/docs/http/authentication
  type: http
  usage: 'Safe to ship in client bundles / browser. Sent as `Authorization: Bearer pk_v1_...` directly from the client. Recommended for prototypes and unscoped public credentials.'
- name: secretKey
  prefix: sk_v1_
  scheme: bearer
  source: https://ai-autocomplete.com/docs/http/authentication
  type: http
  usage: Server-only. Used server-to-server directly, or (recommended) exchanged for a short-lived access token via POST /api/auth/token. Never ship in client code.
- name: accessToken
  prefix: at_v1_
  scheme: bearer
  source: https://ai-autocomplete.com/docs/http/authentication
  type: http
  usage: 'Short-lived token minted from a secret key on the customer''s backend and forwarded to the browser/mobile client. Recommended for production. Response of the token endpoint: { access_token, expires_at (unix seconds), token_type: Bearer }.'
slug: magicx-authentication
source_filename: magicx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://ai-autocomplete.com/docs/http/authentication\ndocs: https://ai-autocomplete.com/docs/http/authentication\nsummary:\n  types: [http]\n  scheme: bearer\n  key_types: [public, secret, access-token]\n  token_mint_endpoint: https://api.ai-autocomplete.com/api/auth/token\ndescription: >-\n  AI Autocomplete authenticates every request to https://api.ai-autocomplete.com with an\n  HTTP Bearer token. Three credential types are issued, all created from the account keys\n  page (https://ai-autocomplete.com/account/keys).\nschemes:\n- name: publicKey\n  type: http\n  scheme: bearer\n  prefix: pk_v1_\n  usage: >-\n    Safe to ship in client bundles / browser. Sent as `Authorization: Bearer pk_v1_...`\n    directly from the client. Recommended for prototypes and unscoped public credentials.\n  source: https://ai-autocomplete.com/docs/http/authentication\n- name: secretKey\n  type: http\n  scheme: bearer\n  prefix: sk_v1_\n  usage:\
  \ >-\n    Server-only. Used server-to-server directly, or (recommended) exchanged for a\n    short-lived access token via POST /api/auth/token. Never ship in client code.\n  source: https://ai-autocomplete.com/docs/http/authentication\n- name: accessToken\n  type: http\n  scheme: bearer\n  prefix: at_v1_\n  usage: >-\n    Short-lived token minted from a secret key on the customer's backend and forwarded to\n    the browser/mobile client. Recommended for production. Response of the token endpoint:\n    { access_token, expires_at (unix seconds), token_type: Bearer }.\n  source: https://ai-autocomplete.com/docs/http/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magicx/refs/heads/main/authentication/magicx-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- AI
- Autocomplete
- Developer Tools
- SDK
- Natural Language
- Productivity
- Machine Learning
---
