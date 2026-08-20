---
api_key_in:
- header
- query
api_specs:
- filename: serper-autocomplete-api-openapi.yml
  format: yaml
  label: Serper Autocomplete API
  slug: serper-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-autocomplete-api-openapi.yml
- filename: serper-images-api-openapi.yml
  format: yaml
  label: Serper Images API
  slug: serper-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-images-api-openapi.yml
- filename: serper-lens-api-openapi.yml
  format: yaml
  label: Serper Lens API
  slug: serper-lens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-lens-api-openapi.yml
- filename: serper-locations-api-openapi.yml
  format: yaml
  label: Serper Locations API
  slug: serper-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-locations-api-openapi.yml
- filename: serper-maps-api-openapi.yml
  format: yaml
  label: Serper Maps API
  slug: serper-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-maps-api-openapi.yml
- filename: serper-news-api-openapi.yml
  format: yaml
  label: Serper News API
  slug: serper-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-news-api-openapi.yml
- filename: serper-patents-api-openapi.yml
  format: yaml
  label: Serper Patents API
  slug: serper-patents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-patents-api-openapi.yml
- filename: serper-places-api-openapi.yml
  format: yaml
  label: Serper Places API
  slug: serper-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-places-api-openapi.yml
- filename: serper-reviews-api-openapi.yml
  format: yaml
  label: Serper Reviews API
  slug: serper-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-reviews-api-openapi.yml
- filename: serper-scholar-api-openapi.yml
  format: yaml
  label: Serper Scholar API
  slug: serper-scholar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-scholar-api-openapi.yml
- filename: serper-search-api-openapi.yml
  format: yaml
  label: Serper Search API
  slug: serper-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-search-api-openapi.yml
- filename: serper-shopping-api-openapi.yml
  format: yaml
  label: Serper Shopping API
  slug: serper-shopping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-shopping-api-openapi.yml
- filename: serper-videos-api-openapi.yml
  format: yaml
  label: Serper Videos API
  slug: serper-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-videos-api-openapi.yml
- filename: serper-webpage-scrape-api-openapi.yml
  format: yaml
  label: Serper Webpage Scrape API
  slug: serper-webpage-scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-webpage-scrape-api-openapi.yml
auth_types:
- apiKey
description: Serper uses a single static API key. The documented path is an X-API-KEY request header on a POST. Serper's own playground can also emit the call as a GET with the key in an `apiKey` query-string parameter — a second, weaker convention that puts the credential in the URL. There is no OAuth, no OIDC, no scopes, no token exchange and no expiry. Keys are created and revoked in the account dashboard at https://serper.dev/api-keys, which supports multiple named keys per account.
kind: authentication
layout: security
method: searched
name: Serper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Serper secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Serper
provider_slug: serper
scheme_count: 2
schemes:
- description: 'Primary scheme. Sent with Content-Type: application/json on a POST to the search or scrape host.'
  in: header
  method: searched
  name: apiKeyHeader
  parameter: X-API-KEY
  sources:
  - https://serper.dev/_next/static/chunks/pages/playground-7ce8960e9fe2fc99.js
  - openapi/serper-search-api-openapi.yml
  type: apiKey
- description: 'Alternative scheme emitted by Serper''s playground when the GET method is selected: every body field is promoted to a query parameter and the key is appended as `apiKey`. Functional but exposes the credential in URLs, proxy logs and browser history. Not represented in any of Serper''s published examples as the default.'
  in: query
  method: searched
  name: apiKeyQuery
  parameter: apiKey
  sources:
  - https://serper.dev/_next/static/chunks/pages/playground-7ce8960e9fe2fc99.js
  type: apiKey
slug: serper-authentication
source_filename: serper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://serper.dev/api-keys, Serper's own playground bundle\n  https://serper.dev/_next/static/chunks/pages/playground-7ce8960e9fe2fc99.js, and live\n  probes of google.serper.dev / scrape.serper.dev / api.serper.dev on 2026-08-13\ndocs: https://serper.dev/api-keys\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2: false\n  oidc: false\n  mtls: false\n  scopes: none\ndescription: >-\n  Serper uses a single static API key. The documented path is an X-API-KEY request header\n  on a POST. Serper's own playground can also emit the call as a GET with the key in an\n  `apiKey` query-string parameter — a second, weaker convention that puts the credential\n  in the URL. There is no OAuth, no OIDC, no scopes, no token exchange and no expiry.\n  Keys are created and revoked in the account dashboard at https://serper.dev/api-keys,\n  which supports multiple named keys per account.\n\nschemes:\n- name:\
  \ apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: >-\n    Primary scheme. Sent with Content-Type: application/json on a POST to the search or\n    scrape host.\n  method: searched\n  sources:\n  - https://serper.dev/_next/static/chunks/pages/playground-7ce8960e9fe2fc99.js\n  - openapi/serper-search-api-openapi.yml\n\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: >-\n    Alternative scheme emitted by Serper's playground when the GET method is selected:\n    every body field is promoted to a query parameter and the key is appended as\n    `apiKey`. Functional but exposes the credential in URLs, proxy logs and browser\n    history. Not represented in any of Serper's published examples as the default.\n  method: searched\n  sources:\n  - https://serper.dev/_next/static/chunks/pages/playground-7ce8960e9fe2fc99.js\n\nkey_management:\n  console: https://serper.dev/api-keys\n  multiple_keys: true\n  named_keys: true\n \
  \ rotation_policy: not published\n  expiry: none published\n  prefix: none published\n  scoping: >-\n    Keys are not scoped to endpoints or search types. Any key can call any published\n    surface, and any key can spend the whole account credit balance.\n  note: >-\n    Serper's dashboard exposes a /users/api-keys listing and per-key usage logs, so keys\n    can be used as a cost-allocation boundary per team or environment — see\n    finops/serper-finops.yml.\n\nunauthenticated_surface:\n  - url: https://api.serper.dev/locations?q=<term>&limit=25\n    status: 200\n    note: >-\n      Answers without a key. Linked from Serper's playground as the public list of\n      supported location values.\n  - url: https://api.serper.dev/health\n    status: 200\n    note: Public health check.\n\ndenial_behaviour:\n  status: 403\n  body: '{\"message\":\"Unauthorized. Sign up for a free account.\",\"statusCode\":403}'\n  observed: '2026-08-13'\n  note: >-\n    The gateway returns 403 (not 401) and\
  \ returns no WWW-Authenticate header, so a client\n    cannot discover the required scheme from the challenge.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/authentication/serper-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Search
- SERP
- Google Search
- Artificial Intelligence
- LLM
- SEO
- Image
- News
- Maps
- Shopping
- Reviews
- Lens
- Scraping
- Locations
- SERP API
- Web Search
- Agents
- Patents
- Scholar
- Autocomplete
- Places
- Videos
---
