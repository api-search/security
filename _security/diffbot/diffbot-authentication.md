---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: diffbot-extract-openapi.json
  format: json
  label: Diffbot Extract API
  slug: diffbot-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-extract-openapi.json
- filename: diffbot-crawl-openapi.json
  format: json
  label: Diffbot Crawl API
  slug: diffbot-crawl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-crawl-openapi.json
- filename: diffbot-bulk-openapi.json
  format: json
  label: Diffbot Bulk Extract API
  slug: diffbot-bulk-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-bulk-openapi.json
- filename: diffbot-dql-openapi.json
  format: json
  label: Diffbot DQL API
  slug: diffbot-dql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-dql-openapi.json
- filename: diffbot-enhance-openapi.json
  format: json
  label: Diffbot Enhance API
  slug: diffbot-enhance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-enhance-openapi.json
- filename: diffbot-natural-language-openapi.json
  format: json
  label: Diffbot Natural Language API
  slug: diffbot-natural-language-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-natural-language-openapi.json
- filename: diffbot-web-search-openapi.json
  format: json
  label: Diffbot Web Search API
  slug: diffbot-web-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-web-search-openapi.json
- filename: diffbot-account-openapi.json
  format: json
  label: Diffbot Account API
  slug: diffbot-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/_original/diffbot-account-openapi.json
- filename: diffbot-knowledge-graph-api-openapi.yml
  format: yaml
  label: Diffbot Knowledge Graph API
  slug: diffbot-knowledge-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/openapi/diffbot-knowledge-graph-api-openapi.yml
auth_types:
- apiKey
- http
description: One credential covers the whole Diffbot estate, but it is presented two different ways. Six of seven surfaces take it as a `token` query parameter; the Web Search API takes the same value as an HTTP Bearer header. There is no OAuth, no OIDC, and no scope system.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Diffbot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Diffbot secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Diffbot
provider_slug: diffbot
scheme_count: 3
schemes:
- applies_to:
  - Extract APIs (https://api.diffbot.com/v3)
  - Crawl API (https://api.diffbot.com/v3)
  - Bulk Extract API (https://api.diffbot.com/v3)
  - Account API (https://api.diffbot.com/v4)
  - DQL API (https://kg.diffbot.com)
  - ENHANCE API (https://kg.diffbot.com)
  description: Your Diffbot API token.
  in: query
  name: tokenscheme
  parameter: token
  sources:
  - openapi/_original/diffbot-extract-openapi.json
  - openapi/_original/diffbot-crawl-openapi.json
  - openapi/_original/diffbot-bulk-openapi.json
  - openapi/_original/diffbot-account-openapi.json
  - openapi/_original/diffbot-dql-openapi.json
  - openapi/_original/diffbot-enhance-openapi.json
  type: apiKey
- applies_to:
  - Natural Language API (https://nl.diffbot.com)
  in: query
  name: DiffbotToken
  note: Same credential, different scheme name — the Natural Language contract is still Swagger 2.0 and names its securityDefinition DiffbotToken.
  parameter: token
  sources:
  - openapi/_original/diffbot-natural-language-openapi.json
  type: apiKey
- applies_to:
  - Web Search API (https://llm.diffbot.com/api/v1/web_search)
  - Diffbot LLM (https://llm.diffbot.com/v1)
  description: Diffbot API Token
  header: Authorization
  name: Authorization
  note: 'THE DIVERGENCE. Same token value, carried as `Authorization: Bearer <token>` instead of ?token=. Confirmed in the published contract and in the curl example at https://www.diffbot.com/docs/web-search/get. An agent that hard-codes the query parameter across the estate will get a 401 on Web Search and on the LLM endpoint.'
  scheme: bearer
  sources:
  - openapi/_original/diffbot-web-search-openapi.json
  type: http
slug: diffbot-authentication
source_filename: diffbot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://www.diffbot.com/docs/authentication, https://www.diffbot.com/docs/account-billing/multiple-tokens,\n  and the securitySchemes blocks of the eight first-party OpenAPI documents in\n  openapi/_original/ (harvested from https://www.diffbot.com/openapi/*.json).\ndocs: https://www.diffbot.com/docs/authentication\nprovider: Diffbot\nproviderId: diffbot\ndescription: >-\n  One credential covers the whole Diffbot estate, but it is presented two different ways.\n  Six of seven surfaces take it as a `token` query parameter; the Web Search API takes the\n  same value as an HTTP Bearer header. There is no OAuth, no OIDC, and no scope system.\nsummary:\n  types:\n    - apiKey\n    - http\n  api_key_in:\n    - query\n  http_schemes:\n    - bearer\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\nschemes:\n  - name: tokenscheme\n    type: apiKey\n    in: query\n    parameter: token\n    description:\
  \ Your Diffbot API token.\n    applies_to:\n      - Extract APIs (https://api.diffbot.com/v3)\n      - Crawl API (https://api.diffbot.com/v3)\n      - Bulk Extract API (https://api.diffbot.com/v3)\n      - Account API (https://api.diffbot.com/v4)\n      - DQL API (https://kg.diffbot.com)\n      - ENHANCE API (https://kg.diffbot.com)\n    sources:\n      - openapi/_original/diffbot-extract-openapi.json\n      - openapi/_original/diffbot-crawl-openapi.json\n      - openapi/_original/diffbot-bulk-openapi.json\n      - openapi/_original/diffbot-account-openapi.json\n      - openapi/_original/diffbot-dql-openapi.json\n      - openapi/_original/diffbot-enhance-openapi.json\n  - name: DiffbotToken\n    type: apiKey\n    in: query\n    parameter: token\n    applies_to:\n      - Natural Language API (https://nl.diffbot.com)\n    sources:\n      - openapi/_original/diffbot-natural-language-openapi.json\n    note: >-\n      Same credential, different scheme name — the Natural Language contract is\
  \ still\n      Swagger 2.0 and names its securityDefinition DiffbotToken.\n  - name: Authorization\n    type: http\n    scheme: bearer\n    header: Authorization\n    description: Diffbot API Token\n    applies_to:\n      - Web Search API (https://llm.diffbot.com/api/v1/web_search)\n      - Diffbot LLM (https://llm.diffbot.com/v1)\n    sources:\n      - openapi/_original/diffbot-web-search-openapi.json\n    note: >-\n      THE DIVERGENCE. Same token value, carried as `Authorization: Bearer <token>` instead\n      of ?token=. Confirmed in the published contract and in the curl example at\n      https://www.diffbot.com/docs/web-search/get. An agent that hard-codes the query\n      parameter across the estate will get a 401 on Web Search and on the LLM endpoint.\ntoken_management:\n  issuance: >-\n    A token is created on registration; a free one at https://app.diffbot.com/get-started.\n  dashboard: https://app.diffbot.com/\n  child_tokens: true\n  child_tokens_note: >-\n    Additional tokens\
  \ can be generated under a parent token, so usage can be segmented per\n    application or team. https://www.diffbot.com/docs/account-billing/multiple-tokens\n  labelling_and_disabling: true\n  labelling_note: >-\n    Tokens can be labelled and disabled from the dashboard — shipped 2025-06-30 per the\n    changelog. This is the closest thing to a revocation control.\n  rotation_policy_published: false\n  expiry: none\n  introspection_endpoint: >-\n    GET https://api.diffbot.com/v4/account returns token details and usage\n    (operationId `account`, openapi/_original/diffbot-account-openapi.json).\nsdk_resolution:\n  order:\n    - explicit token argument\n    - DIFFBOT_API_TOKEN environment variable\n    - a DIFFBOT_API_TOKEN=... line in ~/.diffbot/credentials\n  note: >-\n    diffbot-python's resolve_token() and @diffbot/typescript's resolveTokenFromEnv() share\n    this order, and the CLI uses the same path. Diffbot documents chmod 600 on the\n    credentials file.\nrisks:\n  - id: token-in-query-string\n\
  \    severity: medium\n    finding: >-\n      Six of seven surfaces carry the credential in the URL, so it is exposed to proxy logs,\n      server access logs, browser history and Referer headers. Diffbot's own documentation\n      examples show the token inline in curl URLs.\n    mitigation: >-\n      Use child tokens scoped per application and disable them from the dashboard when\n      leaked; there is no scope system to limit blast radius.\n  - id: no-scopes\n    severity: medium\n    finding: >-\n      A token is all-or-nothing across Extract, Crawl, Bulk, Knowledge Graph, Natural\n      Language, Web Search and Account. There is no read-only credential, so an agent given a\n      token to run searches can also delete crawl jobs — an irreversible action per\n      conventions/diffbot-conventions.yml.\n  - id: no-oauth\n    severity: low\n    finding: >-\n      No delegated-authorization path exists, so Diffbot cannot be integrated on behalf of a\n      third-party user without sharing\
  \ that user's raw token. No /.well-known/\n      openid-configuration or oauth-authorization-server on any host — see\n      well-known/diffbot-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/authentication/diffbot-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Extraction
- Harvesting
- Scraping
- Web
- Knowledge Graph
- Crawling
- Web Search
- Natural Language
- Entity Resolution
- AI
---
