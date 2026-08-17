---
api_key_in: []
api_specs:
- filename: crawlgraph-v1-openapi.yml
  format: yaml
  label: CrawlGraph REST API v1
  slug: crawlgraph-rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlgraph/refs/heads/main/openapi/crawlgraph-v1-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Crawlgraph Authentication
name_suffix: Authentication
oauth_flows: []
overview: CrawlGraph secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CrawlGraph
provider_slug: crawlgraph
scheme_count: 1
schemes:
- description: Every request to /api/v1/* needs a bearer token in the Authorization header. Keys are prefixed cg_live_ and are roughly 52 characters long.
  format: Bearer cg_live_<key>
  header: Authorization
  in: header
  key_length: ~52 characters
  key_prefix: cg_live_
  name: bearerAuth
  scheme: bearer
  sources:
  - https://crawlgraph.com/docs/api
  - openapi/crawlgraph-v1-openapi.yml
  type: http
slug: crawlgraph-authentication
source_filename: crawlgraph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://crawlgraph.com/docs/api\nalso_derived_from: openapi/crawlgraph-v1-openapi.yml\nnote: >-\n  The upstream OpenAPI (https://crawlgraph.com/api/v1/openapi.json) declares NO\n  components.securitySchemes and no security requirement — a real gap, since every /api/v1/*\n  route except free-key rejects an unauthenticated call with 401. The scheme below is taken from\n  section 2 (\"Authentication\") of the published docs and confirmed by live probe: an anonymous\n  GET https://crawlgraph.com/api/v1/releases returns 401. The refined spec in openapi/ adds the\n  missing bearerAuth scheme; the fix is also expressed as an Overlay in overlays/.\n\nsummary:\n  types: [http]\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\n\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer cg_live_<key>'\n    key_prefix: cg_live_\n   \
  \ key_length: ~52 characters\n    description: >-\n      Every request to /api/v1/* needs a bearer token in the Authorization header. Keys are\n      prefixed cg_live_ and are roughly 52 characters long.\n    sources:\n      - https://crawlgraph.com/docs/api\n      - openapi/crawlgraph-v1-openapi.yml\n\nkey_management:\n  self_service: true\n  free_key_endpoint: POST /api/v1/free-key\n  free_key_note: >-\n    The one unauthenticated route. Takes an email address and mails a free-tier key (15 backlink\n    calls/month). No card, no signup, one active key per email. The key is NEVER returned in the\n    HTTP response — only by email.\n  paid_key_console: https://crawlgraph.com/account\n  max_active_keys: 10\n  labels_supported: true\n  shown_once: true\n  recovery: none\n  rotation: revoke and create a new key\n  note: >-\n    The full key is shown only once at creation; there is no recovery path. Up to 10 active keys\n    per user, each labelable (e.g. \"production\", \"n8n-bot\").\n\n\
  tier_gating:\n  - tier: free\n    quota: 15 backlink calls / month\n    tools: [backlinks, releases]\n    note: Free keys can call backlinks. Gap analysis and outreach targets are rejected.\n  - tier: lifetime\n    price: $99 one-time\n    quota: 1,000 backlink calls + 50 gap jobs / month\n    tools: [backlinks, releases, gap_analysis, gap_outreach_targets]\n\nfailure_modes:\n  - code: auth_missing\n    status: 401\n    meaning: Authorization header missing or malformed.\n  - code: auth_invalid\n    status: 401\n    meaning: Key unknown, revoked, or owner refunded.\n\nmcp:\n  shares_credential: true\n  env: CRAWLGRAPH_API_KEY\n  note: >-\n    The hosted MCP server at https://crawlgraph.com/mcp uses the same bearer key and the same\n    quotas as the HTTP API. tools/list is answerable anonymously; tool invocation is not.\n\nx-evidence:\n  - {url: 'https://crawlgraph.com/api/v1/releases', status: 401, note: anonymous GET rejected}\n  - {url: 'https://crawlgraph.com/api/v1/openapi.json',\
  \ status: 200, note: spec served anonymously but declares no securitySchemes}\n  - {url: 'https://crawlgraph.com/docs/api', status: 200, note: section 2 documents the bearer scheme and cg_live_ prefix}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crawlgraph/refs/heads/main/authentication/crawlgraph-authentication.yml
summary_line: http · 1 scheme
tags:
- SEO
- backlink-intelligence
- martech
- competitive-intelligence
- web-data
- Common-Crawl
- link-building
- developer-tools
- API
- MCP
---
