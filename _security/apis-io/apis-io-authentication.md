---
api_key_in:
- header
api_specs:
- filename: apis-io-apis-api-openapi.yml
  format: yaml
  label: APIs.io APIs API
  slug: apis-io-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-apis-api-openapi.yml
- filename: apis-io-areas-api-openapi.yml
  format: yaml
  label: APIs.io Areas API
  slug: apis-io-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-areas-api-openapi.yml
- filename: apis-io-artifact-types-api-openapi.yml
  format: yaml
  label: APIs.io Artifact Types API
  slug: apis-io-artifact-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-artifact-types-api-openapi.yml
- filename: apis-io-industries-api-openapi.yml
  format: yaml
  label: APIs.io Industries API
  slug: apis-io-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-industries-api-openapi.yml
- filename: apis-io-insights-api-openapi.yml
  format: yaml
  label: APIs.io Insights API
  slug: apis-io-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-insights-api-openapi.yml
- filename: apis-io-providers-api-openapi.yml
  format: yaml
  label: APIs.io Providers API
  slug: apis-io-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-providers-api-openapi.yml
- filename: apis-io-ratings-api-openapi.yml
  format: yaml
  label: APIs.io Ratings API
  slug: apis-io-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-ratings-api-openapi.yml
- filename: apis-io-regions-api-openapi.yml
  format: yaml
  label: APIs.io Regions API
  slug: apis-io-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-regions-api-openapi.yml
- filename: apis-io-search-api-openapi.yml
  format: yaml
  label: APIs.io Search API
  slug: apis-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-search-api-openapi.yml
- filename: apis-io-synthesis-api-openapi.yml
  format: yaml
  label: APIs.io Synthesis API
  slug: apis-io-synthesis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-synthesis-api-openapi.yml
- filename: apis-io-tags-api-openapi.yml
  format: yaml
  label: APIs.io Tags API
  slug: apis-io-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Apis Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIs.io secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: APIs.io
provider_slug: apis-io
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  required: false
  sources:
  - openapi/_original/apis-io-v1-openapi.yml
  type: apiKey
- in: header
  name: api_key
  note: The refined per-tag specs spell the header lowercase (`x-api-key`); the v1 contract spells it `X-API-Key`. HTTP header names are case-insensitive, so both work.
  parameter: x-api-key
  required: false
  sources:
  - openapi/apis-io-apis-api-openapi.yml
  - openapi/apis-io-areas-api-openapi.yml
  - openapi/apis-io-artifact-types-api-openapi.yml
  - openapi/apis-io-industries-api-openapi.yml
  - openapi/apis-io-insights-api-openapi.yml
  - openapi/apis-io-providers-api-openapi.yml
  - openapi/apis-io-ratings-api-openapi.yml
  - openapi/apis-io-regions-api-openapi.yml
  - openapi/apis-io-search-api-openapi.yml
  - openapi/apis-io-synthesis-api-openapi.yml
  - openapi/apis-io-tags-api-openapi.yml
  type: apiKey
slug: apis-io-authentication
source_filename: apis-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: searched\nsource: https://apis.io/developer/authentication\ndocs: https://apis.io/developer/authentication\nplans_docs: https://apis.io/developer/plans\nderived_from: openapi/*.yml + openapi/_original/apis-io-v1-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  required: false\n  read_only: true\nmodel: >-\n  v1 is open and read-only — every endpoint is a GET, no endpoint mutates the catalog, and\n  anonymous requests succeed on the Free tier. The OpenAPI declares an `ApiKeyAuth` apiKey scheme\n  that the docs describe as \"API-key-ready\": declared so metering and higher rate tiers can be\n  introduced without a breaking change. In practice a key IS already honoured — GitHub login\n  issues a free Starter key, and Pro/Business keys unlock the Industries, Regions, Ratings,\n  Insights-depth, Saved Workspace and Synthesis operations.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n\
  \  required: false\n  sources:\n  - openapi/_original/apis-io-v1-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  required: false\n  sources:\n  - openapi/apis-io-apis-api-openapi.yml\n  - openapi/apis-io-areas-api-openapi.yml\n  - openapi/apis-io-artifact-types-api-openapi.yml\n  - openapi/apis-io-industries-api-openapi.yml\n  - openapi/apis-io-insights-api-openapi.yml\n  - openapi/apis-io-providers-api-openapi.yml\n  - openapi/apis-io-ratings-api-openapi.yml\n  - openapi/apis-io-regions-api-openapi.yml\n  - openapi/apis-io-search-api-openapi.yml\n  - openapi/apis-io-synthesis-api-openapi.yml\n  - openapi/apis-io-tags-api-openapi.yml\n  note: >-\n    The refined per-tag specs spell the header lowercase (`x-api-key`); the v1 contract spells it\n    `X-API-Key`. HTTP header names are case-insensitive, so both work.\nissuance:\n  method: github-oauth\n  url: https://apis.io/developer/plans\n  note: Log in with GitHub to be issued a free Starter key instantly;\
  \ upgrade via Stripe Checkout.\ntiers:\n- tier: Free\n  auth: none (anonymous)\n  price: $0\n  rate_limit: 5 req/s\n  daily_quota: 1000\n- tier: Starter\n  auth: GitHub login\n  price: $0\n  rate_limit: 20 req/s\n  daily_quota: 10000\n- tier: Pro\n  auth: GitHub login\n  price: $49/mo\n  rate_limit: 100 req/s\n  daily_quota: 100000\n- tier: Business\n  auth: GitHub login\n  price: $199/mo\n  rate_limit: 400 req/s\n  daily_quota: 1000000\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes:\n  present: false\n  reason: apiKey auth only — there is no OAuth scope surface to record.\ncors:\n  allow_origin: '*'\n  allow_headers: [content-type, x-api-key]\n  allow_methods: [GET, OPTIONS]\nmcp_authentication:\n  url: https://apis.io/mcp\n  anonymous_tools_list: true\n  gate: >-\n    Pro-tier tools are listed anonymously but return HTTP 402 `upgrade_required` when called\n    without a paid key.\n  oauth_discovery:\n    /.well-known/oauth-authorization-server: 404\n    /.well-known/oauth-protected-resource:\
  \ 404\nx-evidence:\n  fetched: '2026-08-10'\n  probes:\n  - url: https://apis.io/api/v1/search?q=weather&limit=1\n    http_status: 200\n    note: anonymous, no key\n  - url: https://apis.io/api/v1/ratings\n    http_status: 402\n    note: anonymous — tier gate\n  - url: https://apis.io/developer/authentication\n    http_status: 200\n  - url: https://apis.io/developer/plans\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/authentication/apis-io-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engines
- API Catalog
- Agent Discovery
- MCP
- Agent Skills
- OpenAPI
- API Governance
---
