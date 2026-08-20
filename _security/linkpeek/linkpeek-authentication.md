---
api_key_in:
- query
api_specs:
- filename: linkpeek-favicon-api-openapi.yml
  format: yaml
  label: LinkPeek Favicon API
  slug: linkpeek-favicon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-favicon-api-openapi.yml
- filename: linkpeek-link-preview-api-openapi.yml
  format: yaml
  label: LinkPeek Link Preview API
  slug: linkpeek-link-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-link-preview-api-openapi.yml
- filename: linkpeek-meta-tags-api-openapi.yml
  format: yaml
  label: LinkPeek Meta Tags API
  slug: linkpeek-meta-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-meta-tags-api-openapi.yml
- filename: linkpeek-qr-code-api-openapi.yml
  format: yaml
  label: LinkPeek QR Code API
  slug: linkpeek-qr-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-qr-code-api-openapi.yml
- filename: linkpeek-system-api-openapi.yml
  format: yaml
  label: LinkPeek System API
  slug: linkpeek-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-system-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Linkpeek Authentication
name_suffix: Authentication
oauth_flows: []
overview: LinkPeek secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LinkPeek
provider_slug: linkpeek
scheme_count: 1
schemes:
- description: 'Optional API key for Trial/Pro tiers (lifts daily quota to 50,000).

    Obtain via `/api/key?email=` (free 14-day trial) or

    `/api/subscribe?email=` (Pro, $1/mo). Free tier requires no key.'
  in: query
  key_prefix: lp_pro_
  name: ApiKeyAuth
  parameter: key
  required: false
  sources:
  - openapi/linkpeek-openapi-original.yml
  type: apiKey
slug: linkpeek-authentication
source_filename: linkpeek-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/linkpeek-openapi-original.yml\ndocs: https://147.15.103.217.sslip.io/openapi.yaml\ndocs_additional:\n  - https://github.com/dcn13l/hermes-autonomia\n  - https://147.15.103.217.sslip.io/api/pricing\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  anonymous_tier: true\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  required: false\n  key_prefix: lp_pro_\n  description: |-\n    Optional API key for Trial/Pro tiers (lifts daily quota to 50,000).\n    Obtain via `/api/key?email=` (free 14-day trial) or\n    `/api/subscribe?email=` (Pro, $1/mo). Free tier requires no key.\n  sources:\n  - openapi/linkpeek-openapi-original.yml\nanonymous_access:\n  supported: true\n  metering: per-source-ip\n  daily_limit: 100\n  note: >-\n    The spec's top-level `security` is `[{}, {ApiKeyAuth: []}]` — the empty requirement makes\n    anonymous access a first-class, declared\
  \ mode rather than an accident. There is no signup.\nkey_issuance:\n  trial: 'GET /api/key?email=<address> — 14-day key, no card, auto-expires to Free'\n  pro: 'GET /api/subscribe?email=<address> — non-expiring key plus a PayPal payment link, $1/month'\n  validation: 'GET /api/validate-key?key=<key> (live route; not in the published OpenAPI)'\n  self_serve: true\n  note: >-\n    Both issuance operations are side-effecting `GET` requests with no idempotency contract — see\n    conventions/linkpeek-conventions.yml.\nweaknesses:\n  - >-\n    The key is carried on the query string, so it is exposed to proxy logs, browser history and\n    referrer headers. The spec documents no header alternative, although the live CORS policy\n    advertises `X-API-Key` as an allowed request header.\n  - >-\n    No 401 or 403 response is documented for any operation, so an invalid or expired key has no\n    published contract.\n  - No scopes, no permissions model, no token expiry semantics beyond the 14-day\
  \ trial window.\n  - No OAuth 2.0, no OIDC, no mTLS. /.well-known/openid-configuration and /.well-known/oauth-authorization-server both returned 404.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/authentication/linkpeek-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Screenshots
- webpage-capture
- website-thumbnails
- Image-Generation
- Rendering
- web-scraping-adjacent
- Developer Tools
- Software-as-a-Service
- rest-image-api
- Utility API
- URL Metadata
- Link Preview
- OpenGraph
- QR Code Generation
- DNS
- WHOIS
- SSL
- Web Security Scanning
- IP Geolocation
- Data Conversion
- LLM-Compatible API
- API Utilities
- dns-whois
- openai-compatible-llm
---
