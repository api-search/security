---
api_key_in:
- query
api_specs:
- filename: debounce-validation-api-openapi.yml
  format: yaml
  label: DeBounce Validation API
  slug: debounce-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-validation-api-openapi.yml
- filename: debounce-bulk-api-openapi.yml
  format: yaml
  label: DeBounce Bulk API
  slug: debounce-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-bulk-api-openapi.yml
- filename: debounce-data-api-openapi.yml
  format: yaml
  label: DeBounce Data API
  slug: debounce-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-data-api-openapi.yml
- filename: debounce-account-api-openapi.yml
  format: yaml
  label: DeBounce Account API
  slug: debounce-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-account-api-openapi.yml
- filename: debounce-disposable-api-openapi.yml
  format: yaml
  label: DeBounce Disposable Detector API
  slug: debounce-disposable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-disposable-api-openapi.yml
auth_types:
- apiKey
description: 'DeBounce authenticates every REST request with an API key passed as the `api` query-string parameter. There are no headers to set, no bearer tokens, no OAuth and no signing — which is exactly why the docs warn that the key must never be placed in client-side code. Two key classes exist with materially different posture: a private key with full account access, and a `public_`-prefixed key scoped to browser use with CORS domain allow-listing and a hard per-IP daily cap. The free Disposable Detector and Logo APIs are unauthenticated entirely. A separate OAuth 2.1 authorization server exists on debounce.com, but it belongs to the WordPress-hosted MCP endpoint, not to the validation API — see scopes/debounce-scopes.yml.'
kind: authentication
layout: security
method: searched
name: Debounce Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeBounce secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DeBounce
provider_slug: debounce
scheme_count: 1
schemes:
- description: API key for authentication
  in: query
  name: ApiKeyQuery
  parameter: api
  sources:
  - openapi/debounce-account-api-openapi.yml
  - openapi/debounce-bulk-api-openapi.yml
  - openapi/debounce-data-api-openapi.yml
  - openapi/debounce-validation-api-openapi.yml
  type: apiKey
slug: debounce-authentication
source_filename: debounce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/ (securitySchemes) + provider docs\ndocs: https://developers.debounce.com/api-concepts/authentication\ndescription: >-\n  DeBounce authenticates every REST request with an API key passed as the `api`\n  query-string parameter. There are no headers to set, no bearer tokens, no OAuth\n  and no signing — which is exactly why the docs warn that the key must never be\n  placed in client-side code. Two key classes exist with materially different\n  posture: a private key with full account access, and a `public_`-prefixed key\n  scoped to browser use with CORS domain allow-listing and a hard per-IP daily\n  cap. The free Disposable Detector and Logo APIs are unauthenticated entirely. A\n  separate OAuth 2.1 authorization server exists on debounce.com, but it belongs\n  to the WordPress-hosted MCP endpoint, not to the validation API — see\n  scopes/debounce-scopes.yml.\n\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n\
  \  oauth2_flows: []\n  unauthenticated_surfaces:\n  - https://disposable.debounce.io\n  - https://logo.debounce.com\n\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api\n  description: API key for authentication\n  sources:\n  - openapi/debounce-account-api-openapi.yml\n  - openapi/debounce-bulk-api-openapi.yml\n  - openapi/debounce-data-api-openapi.yml\n  - openapi/debounce-validation-api-openapi.yml\n\nkey_classes:\n- class: private\n  prefix: null\n  format: 13-character alphanumeric token\n  where: query parameter `api`\n  issued_at: https://app.debounce.io/api\n  scope: full account access — validation, bulk, enrichment, balance, usage\n  limits: 5 concurrent calls; 2 when the enrichment (append) option is enabled\n  docs: https://developers.debounce.com/api-concepts/authentication\n- class: public\n  prefix: public_\n  format: '`public_` prefix followed by the key body'\n  where: query parameter `api`, from browser JavaScript\n  scope: single email validation\
  \ only, from an allow-listed origin\n  cors: the calling domain must be added to the key's approved CORS domain list\n  limits: 20 validations per internet IP address per day\n  docs: https://developers.debounce.com/api-concepts/rate-limiting\n\nfailure_modes:\n- http_status: 401\n  body: '{\"debounce\":{\"error\":\"Wrong API\",\"code\":\"0\"},\"success\":\"0\"}'\n  meaning: API key missing, invalid, or not permitted\n  verified: probed\n  x-evidence:\n    url: https://api.debounce.io/v1/?email=test@example.com\n    fetched: '2026-08-14'\n    http_status: 401\n    note: >-\n      Probed with no api parameter. The live response added a \"loc\" field not\n      present in the published Error schema.\n- http_status: 402\n  meaning: credits exhausted — add credits to continue validating\n- http_status: 403\n  meaning: request not allowed for this API key or operation\n- http_status: 429\n  meaning: concurrency limit (private key) or daily per-IP limit (public key) exceeded\n\nguidance:\n-\
  \ >-\n  The key travels in the URL query string, so it lands in server access logs,\n  browser history, and Referer headers. DeBounce's own docs tell integrators to\n  keep the private key server-side; the `public_` key class exists precisely\n  because the private key cannot be safely exposed.\n- >-\n  There is no key rotation, expiry or scoping mechanism documented beyond the\n  private/public split, and no OAuth path to the validation API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/authentication/debounce-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email Validation
- Email Verification
- Deliverability
- Disposable Email Detection
- MX Records
- Bulk Email Validation
- Data Enrichment
- Syntax Validation
- Reverse Email Lookup
- Logo API
---
