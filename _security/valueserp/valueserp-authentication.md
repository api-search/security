---
api_key_in:
- query
api_specs:
- filename: valueserp-images-api-openapi.yml
  format: yaml
  label: ValueSERP Images API
  slug: valueserp-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valueserp/refs/heads/main/openapi/valueserp-images-api-openapi.yml
- filename: valueserp-news-api-openapi.yml
  format: yaml
  label: ValueSERP News API
  slug: valueserp-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valueserp/refs/heads/main/openapi/valueserp-news-api-openapi.yml
- filename: valueserp-places-api-openapi.yml
  format: yaml
  label: ValueSERP Places API
  slug: valueserp-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valueserp/refs/heads/main/openapi/valueserp-places-api-openapi.yml
- filename: valueserp-product-api-openapi.yml
  format: yaml
  label: ValueSERP Product API
  slug: valueserp-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valueserp/refs/heads/main/openapi/valueserp-product-api-openapi.yml
- filename: valueserp-search-api-openapi.yml
  format: yaml
  label: ValueSERP Search API
  slug: valueserp-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valueserp/refs/heads/main/openapi/valueserp-search-api-openapi.yml
- filename: valueserp-shopping-api-openapi.yml
  format: yaml
  label: ValueSERP Shopping API
  slug: valueserp-shopping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valueserp/refs/heads/main/openapi/valueserp-shopping-api-openapi.yml
auth_types:
- apiKey
description: 'ValueSERP authenticates every request with a single API key passed as the `api_key` QUERY-STRING parameter. That is the whole scheme: no OAuth, no OpenID Connect, no bearer tokens, no HMAC request signing, no mTLS, and no scopes. There is one key type with one level of access — a key that can read can also create batches and destinations and spend the account''s credits.'
kind: authentication
layout: security
method: searched
name: Valueserp Authentication
name_suffix: Authentication
oauth_flows: []
overview: ValueSERP secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ValueSERP
provider_slug: valueserp
scheme_count: 1
schemes:
- applies_to: Every documented endpoint — the real-time Search API, Locations API, Account API, Error Logs API, Batches API and Destinations API.
  description: API key for authentication, passed as the api_key query parameter on every request, e.g. https://api.valueserp.com/search?api_key=YOUR_KEY&q=pizza
  header_alternative: false
  in: query
  name: apiKeyQuery
  obtain: https://app.valueserp.com/signup
  parameter: api_key
  required: true
  sources:
  - openapi/valueserp-search-api-openapi.yml
  - https://docs.trajectdata.com/valueserp/HX_zC2K66qg5OEkKe7g5p
  test_value: demo
  test_value_note: The documentation uses the literal key `demo` in every code sample. See sandbox/valueserp-sandbox.yml.
  type: apiKey
slug: valueserp-authentication
source_filename: valueserp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.trajectdata.com/valueserp/HX_zC2K66qg5OEkKe7g5p (Send Requests),\n  https://docs.trajectdata.com/valueserp/account-api,\n  https://docs.trajectdata.com/valueserp/response-codes — confirmed against the\n  securitySchemes block in openapi/valueserp-search-api-openapi.yml.\ndocs: https://docs.trajectdata.com/valueserp/HX_zC2K66qg5OEkKe7g5p\ndescription: >-\n  ValueSERP authenticates every request with a single API key passed as the\n  `api_key` QUERY-STRING parameter. That is the whole scheme: no OAuth, no\n  OpenID Connect, no bearer tokens, no HMAC request signing, no mTLS, and no\n  scopes. There is one key type with one level of access — a key that can read\n  can also create batches and destinations and spend the account's credits.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth: false\n  oidc: false\n  mtls: false\n  scopes: false\n  key_rotation_documented: false\n  multiple_keys_documented:\
  \ false\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  required: true\n  applies_to: >-\n    Every documented endpoint — the real-time Search API, Locations API, Account\n    API, Error Logs API, Batches API and Destinations API.\n  description: >-\n    API key for authentication, passed as the api_key query parameter on every\n    request, e.g.\n    https://api.valueserp.com/search?api_key=YOUR_KEY&q=pizza\n  test_value: 'demo'\n  test_value_note: >-\n    The documentation uses the literal key `demo` in every code sample. See\n    sandbox/valueserp-sandbox.yml.\n  sources:\n  - openapi/valueserp-search-api-openapi.yml\n  - https://docs.trajectdata.com/valueserp/HX_zC2K66qg5OEkKe7g5p\n  header_alternative: false\n  obtain: https://app.valueserp.com/signup\nfailure_modes:\n  - status: 401\n    meaning: The API key supplied with your request is not valid.\n    note: >-\n      Because the key travels in the query string, a truncated or URL-mangled\n \
  \     key surfaces as a 401 rather than a 400.\n  - status: 402\n    meaning: >-\n      The key is valid but the account has run out of credits, or there is a\n      payment problem. Authentication and authorization-to-spend are separate\n      failures here.\nrisks:\n  - >-\n    KEY IN THE URL. The api_key is part of the request URI, so it is written to\n    proxy logs, load-balancer access logs, browser history and any referrer\n    header by default. No header-based alternative is documented, so a caller\n    cannot avoid this.\n  - >-\n    NO SCOPES. One key grants the full surface. There is no read-only key, no\n    per-endpoint restriction, and no way to issue a limited key to a\n    contractor or a client-side process.\n  - >-\n    NO DOCUMENTED ROTATION. The docs describe no key rotation, expiry, or\n    multi-key workflow, so there is no published way to roll a leaked key\n    without a support conversation.\n  - >-\n    A leaked key is directly monetizable — it spends the account's\
  \ purchased\n    credits — which raises the practical impact of the two risks above.\nmitigations:\n  - >-\n    Proxy ValueSERP calls server-side; never place a ValueSERP key in\n    client-side code, where the URL is trivially readable.\n  - >-\n    Poll the free GET /account endpoint for credits_remaining to detect\n    unexpected consumption early. It is the only abuse signal available.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valueserp/refs/heads/main/authentication/valueserp-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- SERP
- Search Engine Results
- Google Search
- Search API
- SEO
- Web Scraping
- Shopping Results
- News Search
- Image Search
- Local Search
- Places
- Data API
---
