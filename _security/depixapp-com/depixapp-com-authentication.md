---
anonymous_access: false
api_key_in: []
api_specs:
- filename: depixapp-com-account-api-openapi.yml
  format: yaml
  label: DePix App Account API
  slug: depixapp-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-account-api-openapi.yml
- filename: depixapp-com-agents-api-openapi.yml
  format: yaml
  label: DePix App Agents API
  slug: depixapp-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-agents-api-openapi.yml
- filename: depixapp-com-checkouts-api-openapi.yml
  format: yaml
  label: DePix App Checkouts API
  slug: depixapp-com-checkouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-checkouts-api-openapi.yml
- filename: depixapp-com-merchant-api-openapi.yml
  format: yaml
  label: DePix App Merchant API
  slug: depixapp-com-merchant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-merchant-api-openapi.yml
- filename: depixapp-com-meta-api-openapi.yml
  format: yaml
  label: DePix App Meta API
  slug: depixapp-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-meta-api-openapi.yml
- filename: depixapp-com-pay-api-openapi.yml
  format: yaml
  label: DePix App Pay API
  slug: depixapp-com-pay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-pay-api-openapi.yml
- filename: depixapp-com-products-api-openapi.yml
  format: yaml
  label: DePix App Products API
  slug: depixapp-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-products-api-openapi.yml
- filename: depixapp-com-public-api-openapi.yml
  format: yaml
  label: DePix App Public API
  slug: depixapp-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-public-api-openapi.yml
- filename: depixapp-com-support-api-openapi.yml
  format: yaml
  label: DePix App Support API
  slug: depixapp-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-support-api-openapi.yml
auth_types:
- http
- signed-request
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: DePix App Authentication
name_suffix: Authentication
oauth_flows: []
overview: DePix App secures its APIs with http and signed-request across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DePix App
provider_slug: depixapp-com
scheme_count: 3
schemes:
- description: 'Authorization: Bearer sk_live_<key> (production) or sk_test_<key> (sandbox). Maximum of 5 live keys and 5 test keys active per account. Keys carry immutable scopes (merchant_read, merchant_write, wallet_read, wallet_write); wallet_write keys carry mandatory spending limits. Key shown only once at creation. sk_live_ keys require manual approval ("Solicitar acesso").'
  key_prefixes:
  - sk_live_
  - sk_test_
  name: apiKey
  scheme: bearer
  sources:
  - openapi/depixapp-com-openapi.yml
  - https://depixapp.com/docs/en/#auth
  type: http
- algorithm: Ed25519
  constraints: nonce single-use, valid ~11 min; timestamp within ±300s of server time
  declared_in_openapi: false
  description: The /api/agents/* endpoints do not use a static API key; every request is signed with the account's Ed25519 key. Canonical string (newline-joined) = depix-agent-auth:v1, api.depixapp.com, METHOD, path-without-query, timestamp, nonce, sha256hex(raw body).
  errors:
  - agent_invalid_signature
  - agent_signature_expired
  - agent_replay_detected
  - agent_unknown_key
  headers:
  - x-agent-public-key
  - x-agent-signature
  - x-agent-nonce
  - x-agent-timestamp
  name: agentSignedRequest
  sources:
  - https://depixapp.com/docs/en/#agents
  type: signed-request
- declared_in_openapi: false
  description: The hosted MCP gateway (https://mcp.depixapp.com/mcp) accepts an OAuth 2.1 connector sign-in (claude.ai / ChatGPT) or a Bearer sk_ key. OAuth sessions are capped to read + merchant scopes and can never move money.
  name: mcpOAuth
  sources:
  - https://depixapp.com/llms.txt
  type: oauth2
slug: depixapp-com-authentication
source_filename: depixapp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://depixapp.com/docs/en/#auth\ndocs: https://depixapp.com/docs/en/#auth\nsummary:\n  types:\n  - http\n  - signed-request\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer sk_live_<key> (production) or sk_test_<key> (sandbox). Maximum of 5 live keys and 5 test keys active per account. Keys carry immutable scopes (merchant_read, merchant_write, wallet_read, wallet_write); wallet_write keys carry mandatory spending limits. Key shown only once at creation. sk_live_ keys require manual approval (\"Solicitar acesso\").'\n  key_prefixes:\n  - sk_live_\n  - sk_test_\n  sources:\n  - openapi/depixapp-com-openapi.yml\n  - https://depixapp.com/docs/en/#auth\n- name: agentSignedRequest\n  type: signed-request\n  algorithm: Ed25519\n  description: The /api/agents/* endpoints do not use a static API key; every request is signed with the account's Ed25519 key. Canonical string (newline-joined)\
  \ = depix-agent-auth:v1, api.depixapp.com, METHOD, path-without-query, timestamp, nonce, sha256hex(raw body).\n  headers:\n  - x-agent-public-key\n  - x-agent-signature\n  - x-agent-nonce\n  - x-agent-timestamp\n  constraints: nonce single-use, valid ~11 min; timestamp within ±300s of server time\n  errors: [agent_invalid_signature, agent_signature_expired, agent_replay_detected, agent_unknown_key]\n  declared_in_openapi: false\n  sources:\n  - https://depixapp.com/docs/en/#agents\n- name: mcpOAuth\n  type: oauth2\n  description: The hosted MCP gateway (https://mcp.depixapp.com/mcp) accepts an OAuth 2.1 connector sign-in (claude.ai / ChatGPT) or a Bearer sk_ key. OAuth sessions are capped to read + merchant scopes and can never move money.\n  declared_in_openapi: false\n  sources:\n  - https://depixapp.com/llms.txt\nwebhook_signing:\n  header: X-DePix-Signature\n  format: t=<unix-ts>,v1=<hmac-sha256-hex>\n  signed_string: timestamp.payload\n  secret: Webhook Secret from My Business\n \
  \ docs: https://depixapp.com/docs/en/#webhook-verify\n"
source_yaml_url: https://artifacts.apis.io/depixapp-com/authentication/depixapp-com-authentication.yml
summary_line: http/signed-request · 3 schemes
tags:
- Company
- Payments
- Pix
- Stablecoins
- Cryptocurrency
- Bitcoin
- Liquid Network
- Brazil
- MCP
---
