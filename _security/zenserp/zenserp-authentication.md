---
api_key_in:
- header
- query
- form
api_specs:
- filename: zenserp-batch-api-openapi.yml
  format: yaml
  label: Zenserp Batch API
  slug: zenserp-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/openapi/zenserp-batch-api-openapi.yml
- filename: zenserp-lists-api-openapi.yml
  format: yaml
  label: Zenserp Lists API
  slug: zenserp-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/openapi/zenserp-lists-api-openapi.yml
- filename: zenserp-search-api-openapi.yml
  format: yaml
  label: Zenserp Search API
  slug: zenserp-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/openapi/zenserp-search-api-openapi.yml
- filename: zenserp-shopping-api-openapi.yml
  format: yaml
  label: Zenserp Shopping Product Page API
  slug: zenserp-shopping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/openapi/zenserp-shopping-api-openapi.yml
- filename: zenserp-trends-api-openapi.yml
  format: yaml
  label: Zenserp Trends API
  slug: zenserp-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/openapi/zenserp-trends-api-openapi.yml
auth_types:
- apiKey
description: 'Zenserp uses a single static API key. Verbatim from the documentation: "Zenserp uses API keys to allow access to the API. You can register a new API key at our developer portal." The key may be presented three ways, and the header form is the one Zenserp recommends. There is no OAuth, no scopes, no token exchange, no test/live key separation and no documented rotation or revocation procedure.'
kind: authentication
layout: security
method: searched
name: Zenserp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zenserp secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zenserp
provider_slug: zenserp
scheme_count: 3
schemes:
- description: 'API key in the `apikey` request header. Zenserp''s own wording: "Zenserp looks for the API key in a header that looks like the following (recommended, works with all requests)."'
  example: 'curl "https://app.zenserp.com/api/v2/search" -H "apikey: <key>"'
  in: header
  name: apiKeyHeader
  parameter: apikey
  recommended: true
  sources:
  - https://app.zenserp.com/documentation#authentification
  - openapi/zenserp-search-api-openapi.yml
  - openapi/zenserp-lists-api-openapi.yml
  - openapi/zenserp-batch-api-openapi.yml
  - openapi/zenserp-trends-api-openapi.yml
  - openapi/zenserp-shopping-api-openapi.yml
  type: apiKey
- applies_to: GET requests
  description: API key as a URL query parameter. Convenient, and the reason a Zenserp key routinely ends up in browser history, proxy logs, referrer headers and server access logs. Prefer the header.
  example: curl "https://app.zenserp.com/api/v2/search?apikey=<key>"
  in: query
  name: apiKeyQuery
  parameter: apikey
  recommended: false
  sources:
  - https://app.zenserp.com/documentation#authentification
  - openapi/zenserp-search-api-openapi.yml
  type: apiKey
- applies_to: POST requests
  description: API key as a multipart/form field on POST requests. Documented only in a curl example. NOT REPRESENTABLE in OpenAPI 3.0 securitySchemes, so it is absent from every OpenAPI in this repo and is carried instead as x-apiKeyFormField in the overlays.
  example: curl "https://app.zenserp.com/api/v2/search" -F "apikey=<key>"
  in: form
  name: apiKeyFormField
  parameter: apikey
  recommended: false
  sources:
  - https://app.zenserp.com/documentation#authentification
  type: apiKey
slug: zenserp-authentication
source_filename: zenserp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://app.zenserp.com/documentation#authentification (read verbatim from the\n  docs SPA bundle /js/app.js), confirmed against a live unauthenticated probe of\n  https://app.zenserp.com/api/v2/search on 2026-08-13; cross-checked against\n  openapi/ securitySchemes\ndocs: https://app.zenserp.com/documentation#authentification\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n    - query\n    - form\n  oauth2: false\n  oidc: false\n  mtls: false\n  environments: 1\n  key_prefix: null\n  rotation_documented: false\ndescription: >-\n  Zenserp uses a single static API key. Verbatim from the documentation: \"Zenserp\n  uses API keys to allow access to the API. You can register a new API key at our\n  developer portal.\" The key may be presented three ways, and the header form is\n  the one Zenserp recommends. There is no OAuth, no scopes, no token exchange, no\n  test/live key separation and no documented rotation\
  \ or revocation procedure.\n\nschemes:\n  - name: apiKeyHeader\n    type: apiKey\n    in: header\n    parameter: apikey\n    recommended: true\n    description: >-\n      API key in the `apikey` request header. Zenserp's own wording: \"Zenserp\n      looks for the API key in a header that looks like the following\n      (recommended, works with all requests).\"\n    example: 'curl \"https://app.zenserp.com/api/v2/search\" -H \"apikey: <key>\"'\n    sources:\n      - https://app.zenserp.com/documentation#authentification\n      - openapi/zenserp-search-api-openapi.yml\n      - openapi/zenserp-lists-api-openapi.yml\n      - openapi/zenserp-batch-api-openapi.yml\n      - openapi/zenserp-trends-api-openapi.yml\n      - openapi/zenserp-shopping-api-openapi.yml\n\n  - name: apiKeyQuery\n    type: apiKey\n    in: query\n    parameter: apikey\n    recommended: false\n    applies_to: GET requests\n    description: >-\n      API key as a URL query parameter. Convenient, and the reason a Zenserp\
  \ key\n      routinely ends up in browser history, proxy logs, referrer headers and\n      server access logs. Prefer the header.\n    example: 'curl \"https://app.zenserp.com/api/v2/search?apikey=<key>\"'\n    sources:\n      - https://app.zenserp.com/documentation#authentification\n      - openapi/zenserp-search-api-openapi.yml\n\n  - name: apiKeyFormField\n    type: apiKey\n    in: form\n    parameter: apikey\n    recommended: false\n    applies_to: POST requests\n    description: >-\n      API key as a multipart/form field on POST requests. Documented only in a\n      curl example. NOT REPRESENTABLE in OpenAPI 3.0 securitySchemes, so it is\n      absent from every OpenAPI in this repo and is carried instead as\n      x-apiKeyFormField in the overlays.\n    example: 'curl \"https://app.zenserp.com/api/v2/search\" -F \"apikey=<key>\"'\n    sources:\n      - https://app.zenserp.com/documentation#authentification\n\nregistration:\n  self_serve: true\n  url: https://app.zenserp.com/register\n\
  \  free_plan_url: https://app.zenserp.com/register?plan=free\n  credit_card_required: false\n  note: 50 free searches per month on signup.\n\nfailure_behavior:\n  status: 403\n  body: '{\"error\": \"No apikey provided.\"}'\n  probed:\n    url: https://app.zenserp.com/api/v2/search?q=test\n    status: 403\n    content_type: application/json\n    fetched: '2026-08-13'\n  note: >-\n    A missing key, a wrong key, an exhausted quota and an unentitled plan all\n    return 403. There is no 401 and no distinct code, so a client cannot\n    programmatically tell \"fix your credentials\" from \"top up your plan\" -- it has\n    to call GET /api/v2/status to find out which.\n\ngaps:\n  - No key prefix or environment marker; a key cannot be identified by inspection.\n  - No test/live separation; the only key is a production key.\n  - No scopes or per-key permissions; every key can call every endpoint the plan entitles.\n  - No documented rotation, expiry or revocation procedure.\n  - No OAuth, no\
  \ OIDC, no service accounts, no delegated access.\n  - Authentication failure is indistinguishable from quota exhaustion (both 403).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/authentication/zenserp-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- SERP
- Search Engine Results
- Google Search
- Web Scraping
- SEO
- Image Search
- News Search
- Shopping Search
- Maps
- YouTube Search
- Bing
- Yandex
- DuckDuckGo
- Geolocation
- Keyword Research
---
