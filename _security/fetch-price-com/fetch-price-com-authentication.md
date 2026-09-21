---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: fetch-price-com-openapi.yml
  format: yaml
  label: fetch-price API
  slug: fetch-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fetch-price-com/refs/heads/main/openapi/fetch-price-com-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fetch Price Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: POLICYANDPLAY LTD secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: POLICYANDPLAY LTD
provider_slug: fetch-price-com
scheme_count: 3
schemes:
- description: fp_-prefixed key issued by POST /api/agents/register. Optional on the free tier (keyless requests are counted per IP); required to use a registered agent's plan quota and BYOK routing. The first-party SDKs send this header.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  required: false
  sources:
  - https://fetch-price.com/docs/#get-key
  - openapi/fetch-price-com-openapi.yml
  type: apiKey
  used_by:
  - npm fetch-price (js/index.js)
  - PyPI fetch-price (python/fetch_price/__init__.py)
- bearerFormat: fp_-prefixed API key
  description: The same key sent as Authorization Bearer, which is how the stdio MCP server and the provider's SKILL.md send it.
  name: BearerAuth
  required: false
  scheme: bearer
  sources:
  - https://fetch-price.com/docs/#get-key
  - openapi/fetch-price-com-openapi.yml
  type: http
  used_by:
  - mcp/fetch_price_mcp.py (FETCH_PRICE_API_KEY)
  - SKILL.md
- description: 'Free tier: no credential; 50 lookups/month and 30 requests/minute counted per IP. Observed 2026-09-19 - unauthenticated GET /health, GET /api/stats and POST /api/query all answered without a challenge.'
  name: anonymous
  required: false
  sources:
  - https://fetch-price.com/docs/#quickstart
  type: none
slug: fetch-price-com-authentication
source_filename: fetch-price-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://fetch-price.com/docs/#get-key\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  anonymous_access: true\n  note: 'Docs: \"The free tier works without authentication (50 lookups/month). Register to get an fp_ key, higher\n    limits, and BYOK affiliate routing ... Send the key on every request as X-API-Key: fp_... (or Authorization:\n    Bearer fp_...).\" One static credential, two carriers. No OAuth, no scopes, no key rotation endpoint. The key\n    is emailed to the registering address by Resend, is never displayed in a public response after issuance, and\n    is revoked by emailing the provider (privacy page). The stdio MCP server reads it from FETCH_PRICE_API_KEY and\n    sends it as Bearer; both SDKs read the same variable and send X-API-Key.'\n  transport: HTTPS only (HSTS on both hosts); header-borne; CORS allows X-API-Key and Authorization from any origin\nschemes:\n- name: ApiKeyAuth\n \
  \ type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: fp_-prefixed key issued by POST /api/agents/register. Optional on the free tier (keyless requests\n    are counted per IP); required to use a registered agent's plan quota and BYOK routing. The first-party SDKs\n    send this header.\n  sources:\n  - https://fetch-price.com/docs/#get-key\n  - openapi/fetch-price-com-openapi.yml\n  required: false\n  used_by:\n  - npm fetch-price (js/index.js)\n  - PyPI fetch-price (python/fetch_price/__init__.py)\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: fp_-prefixed API key\n  description: The same key sent as Authorization Bearer, which is how the stdio MCP server and the provider's SKILL.md\n    send it.\n  sources:\n  - https://fetch-price.com/docs/#get-key\n  - openapi/fetch-price-com-openapi.yml\n  required: false\n  used_by:\n  - mcp/fetch_price_mcp.py (FETCH_PRICE_API_KEY)\n  - SKILL.md\n- name: anonymous\n  type: none\n  required: false\n  description:\
  \ 'Free tier: no credential; 50 lookups/month and 30 requests/minute counted per IP. Observed 2026-09-19\n    - unauthenticated GET /health, GET /api/stats and POST /api/query all answered without a challenge.'\n  sources:\n  - https://fetch-price.com/docs/#quickstart\ndocs: https://fetch-price.com/docs/#get-key\nspec: openapi/fetch-price-com-openapi.yml (API Evangelist-generated from the same docs)\nissuance:\n  operation: POST https://api.fetch-price.com/api/agents/register (operationId registerAgent)\n  required_fields:\n  - name\n  - owner\n  - networks\n  - endpoint\n  response: '{\"agent_id\":\"agent-...\",\"api_key\":\"fp_...\",\"tier\":\"free\",\"query_limit\":50}'\n  delivery: returned once in the response and emailed to owner\n  rotation: none published\n  revocation: by email to the provider - \"If you think a key is compromised, email us and we will revoke it.\"\ntiers:\n  keyless: free tier, quota counted per IP\n  keyed_free: free tier, quota per key\n  keyed_paid: Pro /\
  \ Scale / Trade quotas + BYOK affiliate routing\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fetch-price-com/refs/heads/main/authentication/fetch-price-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Price Comparison
- Product Search
- E-Commerce
- Affiliates
- Marketplace
- Shopping
- eBay
- United Kingdom
- AI Agents
- A2A
- MCP
---
