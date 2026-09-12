---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: apis-io-submit-api-openapi.yml
  format: yaml
  label: APIs.io Submit API
  slug: apisio-submit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-submit-api-openapi.yml
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
- filename: apis-io-cohorts-api-openapi.yml
  format: yaml
  label: APIs.io Cohorts API
  slug: apis-io-cohorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-cohorts-api-openapi.yml
- filename: apis-io-editorial-api-openapi.yml
  format: yaml
  label: APIs.io Editorial API
  slug: apis-io-editorial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-editorial-api-openapi.yml
- filename: apis-io-export-api-openapi.yml
  format: yaml
  label: APIs.io Export API
  slug: apis-io-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-export-api-openapi.yml
- filename: apis-io-resolve-enrich-api-openapi.yml
  format: yaml
  label: APIs.io Resolve & Enrich API
  slug: apis-io-resolve-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-resolve-enrich-api-openapi.yml
- filename: apis-io-saved-workspace-api-openapi.yml
  format: yaml
  label: APIs.io Saved Workspace API
  slug: apis-io-saved-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-saved-workspace-api-openapi.yml
- filename: apis-io-venture-capital-api-openapi.yml
  format: yaml
  label: APIs.io Venture Capital API
  slug: apis-io-venture-capital-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-venture-capital-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Apis Io Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: APIs.io secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
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
source_yaml: "generated: '2026-09-11'\nmethod: searched\nsource: https://apis.io/developer/authentication\ndocs: https://apis.io/developer/authentication\nplans_docs: https://apis.io/developer/plans\nderived_from: openapi/*.yml + openapi/_original/apis-io-v1-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  required: false\n  read_only: false\n  read_only_note: >-\n    Corrected 2026-09-11. The catalog-read surface is still GET-only, but the v1 contract now\n    carries 32 POST and 7 DELETE operations across Provider Control (/providers/{slug}/claim,\n    /facts, /submit, /visibility, /dispute, /correction, /checks, /gaps/report) and Saved\n    Workspace (/me/searches, /me/lists, /me/watch). This file previously asserted read_only: true\n    and oauth2: false; both were true on 2026-08-10 and are not true now.\nmodel: >-\n  v1 is open and read-only — every endpoint is a GET, no endpoint mutates\
  \ the catalog, and\n  anonymous requests succeed on the Free tier. The OpenAPI declares an `ApiKeyAuth` apiKey scheme\n  that the docs describe as \"API-key-ready\": declared so metering and higher rate tiers can be\n  introduced without a breaking change. In practice a key IS already honoured — GitHub login\n  issues a free Starter key, and Pro/Business keys unlock the Industries, Regions, Ratings,\n  Insights-depth, Saved Workspace and Synthesis operations.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  required: false\n  sources:\n  - openapi/_original/apis-io-v1-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  required: false\n  sources:\n  - openapi/apis-io-apis-api-openapi.yml\n  - openapi/apis-io-areas-api-openapi.yml\n  - openapi/apis-io-artifact-types-api-openapi.yml\n  - openapi/apis-io-industries-api-openapi.yml\n  - openapi/apis-io-insights-api-openapi.yml\n  - openapi/apis-io-providers-api-openapi.yml\n\
  \  - openapi/apis-io-ratings-api-openapi.yml\n  - openapi/apis-io-regions-api-openapi.yml\n  - openapi/apis-io-search-api-openapi.yml\n  - openapi/apis-io-synthesis-api-openapi.yml\n  - openapi/apis-io-tags-api-openapi.yml\n  note: >-\n    The refined per-tag specs spell the header lowercase (`x-api-key`); the v1 contract spells it\n    `X-API-Key`. HTTP header names are case-insensitive, so both work.\nissuance:\n  method: github-oauth\n  url: https://apis.io/developer/plans\n  note: Log in with GitHub to be issued a free Starter key instantly; upgrade via Stripe Checkout.\ntiers:\n- tier: Free\n  auth: none (anonymous)\n  price: $0\n  rate_limit: 5 req/s\n  daily_quota: 1000\n- tier: Starter\n  auth: GitHub login\n  price: $0\n  rate_limit: 20 req/s\n  daily_quota: 10000\n- tier: Pro\n  auth: GitHub login\n  price: $49/mo\n  rate_limit: 100 req/s\n  daily_quota: 100000\n- tier: Business\n  auth: GitHub login\n  price: $199/mo\n  rate_limit: 400 req/s\n  daily_quota: 1000000\noauth2:\
  \ true\nopenid_connect: true\nmutual_tls: false\noauth2_server:\n  issuer: https://apis.io\n  metadata_rfc8414: https://apis.io/.well-known/oauth-authorization-server\n  metadata_openid: https://apis.io/.well-known/openid-configuration\n  protected_resource_rfc9728: https://apis.io/.well-known/oauth-protected-resource\n  jwks_uri: https://apis.io/.well-known/jwks.json\n  authorization_endpoint: https://apis.io/api/v1/auth/authorize\n  token_endpoint: https://apis.io/api/v1/auth/token\n  registration_endpoint: https://apis.io/api/v1/auth/register\n  grant_types: [authorization_code, refresh_token, client_credentials]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\n  resource_indicators_supported: true\n  protected_resource: https://apis.io/mcp\n  note: >-\n    RFC 7591 dynamic client registration plus a client_credentials grant means an agent\
  \ can\n    register itself and take a token with no human in the loop. The protected resource named by\n    the RFC 9728 document is the MCP server, not the REST API — a key is optional on /api/v1 and\n    raises the tier rather than granting access.\naauth:\n  document: https://apis.io/.well-known/aauth-resource.json\n  issuer: https://apis.io\n  jwks_uri: https://apis.io/.well-known/jwks.json\n  r3_vocabularies:\n    urn:aauth:vocabulary:openapi: https://apis.io/openapi.json\n    urn:aauth:vocabulary:mcp: https://apis.io/mcp\n  defect: >-\n    The r3_vocabularies OpenAPI pointer https://apis.io/openapi.json returned HTTP 404 when\n    probed on 2026-09-11 (the served document is an HTML shell, 26,159 bytes). The MCP pointer\n    resolves. An AAuth client following the OpenAPI vocabulary URI finds nothing. Recorded here\n    rather than quietly dropped — this is our own document making a claim the host does not honour.\nscopes:\n  present: true\n  artifact: scopes/apis-io-scopes.yml\n\
  \  scopes: [apis:read, apis:pro, offline_access]\ncors:\n  allow_origin: '*'\n  allow_headers: [content-type, x-api-key]\n  allow_methods: [GET, OPTIONS]\nmcp_authentication:\n  url: https://apis.io/mcp\n  anonymous_tools_list: true\n  gate: >-\n    Pro-tier tools are listed anonymously but return HTTP 402 `upgrade_required` when called\n    without a paid key.\n  oauth_discovery:\n    /.well-known/oauth-authorization-server: 200\n    /.well-known/oauth-protected-resource: 200\n    /.well-known/openid-configuration: 200\n    /.well-known/aauth-resource.json: 200\n    checked: '2026-09-11'\n    note: All four 404'd on 2026-08-10 and are served now.\nx-evidence:\n  fetched: '2026-09-11'\n  probes:\n  - url: https://apis.io/.well-known/oauth-authorization-server\n    http_status: 200\n    note: RFC 8414, saved to well-known/apis-io-oauth-authorization-server.json\n  - url: https://apis.io/.well-known/openid-configuration\n    http_status: 200\n    note: saved to well-known/apis-io-openid-configuration.json\n\
  \  - url: https://apis.io/.well-known/oauth-protected-resource\n    http_status: 200\n    note: RFC 9728, resource https://apis.io/mcp\n  - url: https://apis.io/.well-known/aauth-resource.json\n    http_status: 200\n    note: AAuth resource, issuer + jwks_uri present\n  - url: https://apis.io/.well-known/jwks.json\n    http_status: 200\n  - url: https://apis.io/openapi.json\n    http_status: 404\n    note: named by aauth r3_vocabularies; not served\n  - url: https://apis.io/api/v1/\n    http_status: 401\n    note: anonymous call to an undefined endpoint — unauthorized envelope\n  - url: https://apis.io/api/v1/search?q=weather&limit=1\n    http_status: 200\n    note: anonymous, no key (first observed 2026-08-10, re-confirmed 2026-09-11)\n  - url: https://apis.io/api/v1/ratings\n    http_status: 402\n    note: anonymous — tier gate\n  - url: https://apis.io/developer/authentication\n    http_status: 200\n  - url: https://apis.io/developer/plans\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/authentication/apis-io-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
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
