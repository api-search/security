---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: litescrape-apple-api-openapi.yml
  format: yaml
  label: Litescrape Apple API
  slug: litescrape-apple-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-apple-api-openapi.yml
- filename: litescrape-bing-api-openapi.yml
  format: yaml
  label: Litescrape Bing API
  slug: litescrape-bing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-bing-api-openapi.yml
- filename: litescrape-duckduckgo-api-openapi.yml
  format: yaml
  label: Litescrape Duckduckgo API
  slug: litescrape-duckduckgo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-duckduckgo-api-openapi.yml
- filename: litescrape-google-api-openapi.yml
  format: yaml
  label: Litescrape Google API
  slug: litescrape-google-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-google-api-openapi.yml
- filename: litescrape-tripadvisor-api-openapi.yml
  format: yaml
  label: Litescrape Tripadvisor API
  slug: litescrape-tripadvisor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-tripadvisor-api-openapi.yml
- filename: litescrape-yelp-api-openapi.yml
  format: yaml
  label: Litescrape Yelp API
  slug: litescrape-yelp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-yelp-api-openapi.yml
- filename: litescrape-zeroclick-api-openapi.yml
  format: yaml
  label: Litescrape Zeroclick API
  slug: litescrape-zeroclick-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-zeroclick-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Litescrape Authentication
name_suffix: Authentication
oauth_flows: []
overview: Litescrape secures its APIs with http and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Litescrape
provider_slug: litescrape
scheme_count: 4
schemes:
- description: '"Send Authorization: Bearer YOUR_API_KEY in the request headers. Never place your key in the URL or browser bundle." Missing or malformed bearer headers return 401 missing_api_key; invalid keys return 401 invalid_api_key; disabled keys return 403 api_key_disabled (key-status page; 401s observed live with WWW-Authenticate: Bearer). The same key is optional on the hosted MCP server (Authorization: Bearer, or ?api_key= in HTTP mode).'
  docs: https://litescrape.com/docs/key-status
  header: Authorization
  key_prefix: ls_live_
  name: apiKeyBearer
  scheme: bearer
  sources:
  - https://litescrape.com/docs/key-status
  - https://litescrape.com/docs/reference
  type: http
- description: 'Plan access. Calls are sold on plans (credit or subscription), not per call: an unidentified call returns 401 bearer_required with a registration recipe, and an identified call with no covering plan returns 403 plan_required listing the plans that cover it. Reuse your existing agent identity; register only if new (anonymous registration is one free API call; the recipe is at https://agents.litescr'
  name: planAccess
  scheme: bearer
  sources:
  - openapi/litescrape-openapi.yml
  type: http
- description: Signed $0 x402 proof from the 402 challenge
  in: header
  name: sellerAgentX402
  parameter: Payment-Signature
  sources:
  - openapi/litescrape-openapi.yml
  type: apiKey
- description: Signed $0 MPP proof from the 402 challenge
  name: sellerAgentMpp
  scheme: Payment
  sources:
  - openapi/litescrape-openapi.yml
  type: http
slug: litescrape-authentication
source_filename: litescrape-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource:\n- https://litescrape.com/docs/key-status\n- https://litescrape.com/docs/reference\n- openapi/litescrape-openapi.yml (agents.litescrape.com storefront schemes)\n- live 401 probes of https://api.litescrape.com (2026-10-07)\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  primary: Bearer API key (ls_live_ prefix) in the Authorization header against https://api.litescrape.com\n  storefront: The published OpenAPI describes the ZeroClick agent storefront at agents.litescrape.com, whose planAccess bearer\n    token comes from the storefront's own OAuth 2.0 token endpoint (https://agents.litescrape.com/oauth2/token, issuer https://agentauth.zeroclick.io,\n    RFC 9728 protected-resource and RFC 8414 metadata served) and whose quote operation accepts x402 / MPP payment proofs.\n    Those schemes are below as derived.\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  key_prefix: ls_live_\n  header:\
  \ Authorization\n  description: '\"Send Authorization: Bearer YOUR_API_KEY in the request headers. Never place your key in the URL or browser\n    bundle.\" Missing or malformed bearer headers return 401 missing_api_key; invalid keys return 401 invalid_api_key; disabled\n    keys return 403 api_key_disabled (key-status page; 401s observed live with WWW-Authenticate: Bearer). The same key is\n    optional on the hosted MCP server (Authorization: Bearer, or ?api_key= in HTTP mode).'\n  docs: https://litescrape.com/docs/key-status\n  sources:\n  - https://litescrape.com/docs/key-status\n  - https://litescrape.com/docs/reference\n- name: planAccess\n  type: http\n  scheme: bearer\n  description: 'Plan access. Calls are sold on plans (credit or subscription), not per call: an unidentified call returns\n    401 bearer_required with a registration recipe, and an identified call with no covering plan returns 403 plan_required\n    listing the plans that cover it. Reuse your existing agent identity;\
  \ register only if new (anonymous registration is one\n    free API call; the recipe is at https://agents.litescr'\n  sources:\n  - openapi/litescrape-openapi.yml\n- name: sellerAgentX402\n  type: apiKey\n  in: header\n  parameter: Payment-Signature\n  description: Signed $0 x402 proof from the 402 challenge\n  sources:\n  - openapi/litescrape-openapi.yml\n- name: sellerAgentMpp\n  type: http\n  scheme: Payment\n  description: Signed $0 MPP proof from the 402 challenge\n  sources:\n  - openapi/litescrape-openapi.yml\ndocs: https://litescrape.com/docs/key-status\nkey_management:\n  issue: Get your API key at https://litescrape.com (5 free calls on a new visitor key; one free key per browser, 409 otherwise)\n  status: GET /api/keys/status returns remaining_calls, concurrency_limit, status, zdr_enabled, zdr_available\n  settings: 'PATCH /api/keys/zdr {\"zdr_enabled\": true|false} for keys with a paid top-up'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/authentication/litescrape-authentication.yml
summary_line: http/apiKey · 4 schemes
tags:
- Company
- SERP API
- Web Scraping
- Search
- Google Maps
- Reviews
- Web Data
- MCP
---
