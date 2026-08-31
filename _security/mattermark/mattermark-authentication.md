---
api_key_in:
- header
- query
api_specs:
- filename: mattermark-companies-api-openapi.yml
  format: yaml
  label: Mattermark Companies API
  slug: mattermark-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/openapi/mattermark-companies-api-openapi.yml
- filename: mattermark-complex-queries-api-openapi.yml
  format: yaml
  label: Mattermark Complex Queries API
  slug: mattermark-complex-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/openapi/mattermark-complex-queries-api-openapi.yml
- filename: mattermark-funding-events-api-openapi.yml
  format: yaml
  label: Mattermark Funding Events API
  slug: mattermark-funding-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/openapi/mattermark-funding-events-api-openapi.yml
- filename: mattermark-investors-api-openapi.yml
  format: yaml
  label: Mattermark Investors API
  slug: mattermark-investors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/openapi/mattermark-investors-api-openapi.yml
- filename: mattermark-search-api-openapi.yml
  format: yaml
  label: Mattermark Search API
  slug: mattermark-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/openapi/mattermark-search-api-openapi.yml
- filename: mattermark-utilities-api-openapi.yml
  format: yaml
  label: Mattermark Utilities API
  slug: mattermark-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/openapi/mattermark-utilities-api-openapi.yml
auth_types:
- apiKey
- http
description: 'Mattermark authenticates both the REST API (https://api.mattermark.com/) and the GraphQL API (https://eapi.mattermark.com/) with a single static account API key. The key is accepted two ways: as an HTTP Bearer token in the Authorization header (the form the published Swagger definition declares), or as a `key` query-string parameter (documented on the REST getting-started page). There is no OAuth 2.0 or OpenID Connect surface, no scope model, no token exchange and no key rotation or expiry policy in the documentation.'
kind: authentication
layout: security
method: searched
name: Mattermark Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mattermark secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mattermark
provider_slug: mattermark
scheme_count: 2
schemes:
- applies_to:
  - https://api.mattermark.com/
  - https://eapi.mattermark.com/
  description: The security definition declared in the first-party Swagger 2.0 document and applied globally via a root-level `security` requirement, so every one of the 11 operations requires it.
  format: Bearer <api key>
  in: header
  name: APIKeyHeaderParam
  parameter: Authorization
  source: openapi/mattermark-rest-api-openapi.yml
  spec_declared: true
  type: apiKey
- applies_to:
  - https://api.mattermark.com/
  description: '"We look for your API key in the key query parameter or the Authentication header." Every REST example in the docs uses this form (e.g. GET /companies?key=[YOUR KEY]). It is NOT declared in the published Swagger definition, so the specification understates the auth surface.'
  in: query
  name: keyQueryParam
  parameter: key
  risk: Keys passed in a query string are logged by intermediaries, proxies and browser history. The provider documents no rotation path.
  source: https://docs.mattermark.com/rest_api/getting_started/index.html
  spec_declared: false
  type: apiKey
slug: mattermark-authentication
source_filename: mattermark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://docs.mattermark.com/rest_api/getting_started/index.html\ndocs:\n- https://docs.mattermark.com/rest_api/getting_started/index.html\n- https://docs.mattermark.com/graphql_api/getting_started/index.html\n- https://developer.mattermark.com/docs\nspec_source: openapi/mattermark-rest-api-openapi.yml\nsummary:\n  types: [apiKey, http]\n  http_schemes: [bearer]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  oidc: false\ndescription: >-\n  Mattermark authenticates both the REST API (https://api.mattermark.com/) and\n  the GraphQL API (https://eapi.mattermark.com/) with a single static account\n  API key. The key is accepted two ways: as an HTTP Bearer token in the\n  Authorization header (the form the published Swagger definition declares), or\n  as a `key` query-string parameter (documented on the REST getting-started\n  page). There is no OAuth 2.0 or OpenID Connect surface, no scope model, no\n  token exchange and\
  \ no key rotation or expiry policy in the documentation.\nschemes:\n- name: APIKeyHeaderParam\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer <api key>'\n  source: openapi/mattermark-rest-api-openapi.yml\n  spec_declared: true\n  description: >-\n    The security definition declared in the first-party Swagger 2.0 document and\n    applied globally via a root-level `security` requirement, so every one of\n    the 11 operations requires it.\n  applies_to:\n  - https://api.mattermark.com/\n  - https://eapi.mattermark.com/\n- name: keyQueryParam\n  type: apiKey\n  in: query\n  parameter: key\n  source: https://docs.mattermark.com/rest_api/getting_started/index.html\n  spec_declared: false\n  description: >-\n    \"We look for your API key in the key query parameter or the Authentication\n    header.\" Every REST example in the docs uses this form\n    (e.g. GET /companies?key=[YOUR KEY]). It is NOT declared in the published\n    Swagger definition, so the specification\
  \ understates the auth surface.\n  applies_to:\n  - https://api.mattermark.com/\n  risk: >-\n    Keys passed in a query string are logged by intermediaries, proxies and\n    browser history. The provider documents no rotation path.\nkey_provisioning:\n  source: Mattermark account -> API settings page\n  urls:\n  - {url: 'https://mattermark.com/app/account/api', status: 404}\n  - {url: 'https://mattermark.com/app/api_signup', status: 404}\n  sales_contact: sales@mattermark.com\n  note: >-\n    Both credential URLs linked from the documentation return HTTP 404 at probe\n    time, so there is no working self-serve path to obtain a key. Provisioning\n    is effectively sales-gated.\n  entitlement: >-\n    The docs distinguish trial access (max 50 results, no paging) from full\n    \"Enterprise API key\" access.\npublished_credentials:\n- kind: sandbox\n  host: https://eapi-sandbox.mattermark.com\n  scope: GraphQL sandbox, static data, no quota\n  ref: sandbox/mattermark-sandbox.yml\n  note:\
  \ >-\n    A shared non-secret sandbox key is published verbatim in the GraphQL docs.\n    Captured in the sandbox artifact; the host is no longer reachable.\ntransport_security:\n  https_required: true\n  http_supported: false\n  statement: >-\n    \"The Mattermark API is served over HTTPS. To ensure data privacy,\n    unencrypted HTTP is not supported.\"\n  observed: >-\n    Both API hosts reject the TLS handshake with alert 112 (unrecognized_name);\n    no certificate is served for either SNI. See\n    security/mattermark-domain-security.yml.\nnotes:\n- >-\n  Superseded the previous revision, which recorded only the Bearer header form.\n  The `key` query parameter and the spec-declared APIKeyHeaderParam security\n  definition were added after the first-party Swagger document was located at\n  github.com/Mattermark/mattermark-openapi.\n- No OAuth 2.0 / OIDC surface exists, so scopes/ is intentionally not emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/authentication/mattermark-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Business Intelligence
- Company Data
- Investors
- Funding
- Sales Intelligence
- Market Research
---
