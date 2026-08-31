---
api_key_in:
- query
api_specs:
- filename: serpwow-search-api-openapi.yml
  format: yaml
  label: SerpWow Search API
  slug: serpwow-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serpwow/refs/heads/main/openapi/serpwow-search-api-openapi.yml
auth_types:
- apiKey
description: SerpWow authenticates every request with a single `api_key` query-string parameter. There is no header-based alternative, no OAuth, no OIDC and no scope model — the key is the whole authorization surface, and it carries full account authority including the Batches and Destinations write operations.
kind: authentication
layout: security
method: searched
name: Serpwow Authentication
name_suffix: Authentication
oauth_flows: []
overview: SerpWow secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SerpWow
provider_slug: serpwow
scheme_count: 1
schemes:
- applies_to:
  - Search API
  - Account API
  - Batches API
  - Locations API
  - Destinations API
  - Error Logs API
  docs_quote: api_key | required | The API key for your SerpWow account.
  in: query
  name: apiKeyAuth
  parameter: api_key
  required: true
  sources:
  - openapi/serpwow-search-api-openapi.yml
  - https://docs.trajectdata.com/serpwow/search-api/searches/common
  type: apiKey
slug: serpwow-authentication
source_filename: serpwow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: openapi/serpwow-search-api-openapi.yml\ndocs: https://docs.trajectdata.com/serpwow/search-api/searches/common\ndescription: >-\n  SerpWow authenticates every request with a single `api_key` query-string parameter. There is no\n  header-based alternative, no OAuth, no OIDC and no scope model — the key is the whole\n  authorization surface, and it carries full account authority including the Batches and\n  Destinations write operations.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  required: true\n  applies_to:\n  - Search API\n  - Account API\n  - Batches API\n  - Locations API\n  - Destinations API\n  - Error Logs API\n  sources:\n  - openapi/serpwow-search-api-openapi.yml\n  - https://docs.trajectdata.com/serpwow/search-api/searches/common\n  docs_quote:\
  \ 'api_key | required | The API key for your SerpWow account.'\nkey_management:\n  issuance: https://app.serpwow.com/signup\n  dashboard: https://app.serpwow.com/\n  rotation_documented: false\n  multiple_keys_documented: false\n  prefix_scheme: none\n  observed_format: 32-character uppercase hexadecimal\n  observed_format_note: >-\n    Inferred from the provider's own published request examples; the docs do not state a key\n    format contract, so do not validate against it.\n  demo_key: demo\n  demo_key_note: >-\n    A working, publicly documented demo key. See sandbox/serpwow-sandbox.yml — verified live on\n    2026-08-27 against https://api.serpwow.com/live/account.\nverified:\n- url: https://api.serpwow.com/live/search?q=test\n  http_status: 401\n  body: '{\"request_info\":{\"success\":false,\"message\":\"Supplied api_key is not valid\"}}'\n  fetched: '2026-08-27'\n  note: A missing or invalid key returns 401 with the standard error envelope.\n- url: https://api.serpwow.com/live/account?api_key=demo\n\
  \  http_status: 200\n  fetched: '2026-08-27'\n  note: The published demo key authenticates successfully.\nrisks:\n- id: key-in-url\n  description: >-\n    Because the credential travels in the query string it is written into browser history, proxy\n    logs, CDN logs and server access logs by default. Anything that logs full request URLs will\n    capture the key.\n  mitigation: >-\n    Terminate SerpWow calls server-side, redact `api_key` from request logging, and never place\n    the key in a client-side request.\n- id: no-scopes\n  description: >-\n    One key grants every capability, including deleting Batches and Destinations. There is no way\n    to issue a read-only credential for a search-only integration.\n- id: no-documented-rotation\n  description: >-\n    No key rotation or multi-key procedure is documented, so there is no published path to roll a\n    leaked key without an interruption.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serpwow/refs/heads/main/authentication/serpwow-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Search
- SERP
- Web Data
- Scraping
- SEO
- Search Engines
- Google
- E-Commerce
- Market Intelligence
- Data Extraction
---
