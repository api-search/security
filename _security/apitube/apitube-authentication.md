---
anonymous_access: false
api_key_in:
- header
- query
- bearer
api_specs:
- filename: apitube-news-api-openapi.yml
  format: yaml
  label: APITube News API
  slug: apitube-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-news-api-openapi.yml
- filename: apitube-account-api-openapi.yml
  format: yaml
  label: APITube Account API
  slug: apitube-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-account-api-openapi.yml
- filename: apitube-fact-check-api-openapi.yml
  format: yaml
  label: APITube Fact Check API
  slug: apitube-fact-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-fact-check-api-openapi.yml
- filename: apitube-reference-api-openapi.yml
  format: yaml
  label: APITube Reference API
  slug: apitube-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-reference-api-openapi.yml
- filename: apitube-suggest-api-openapi.yml
  format: yaml
  label: APITube Suggest API
  slug: apitube-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-suggest-api-openapi.yml
- filename: apitube-system-api-openapi.yml
  format: yaml
  label: APITube System API
  slug: apitube-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-system-api-openapi.yml
- filename: apitube-utilities-api-openapi.yml
  format: yaml
  label: APITube Utilities API
  slug: apitube-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/openapi/apitube-utilities-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Apitube Authentication
name_suffix: Authentication
oauth_flows: []
overview: APITube secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: APITube
provider_slug: apitube
scheme_count: 2
schemes:
- description: API key passed as a request header
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/apitube-account-api-openapi.yml
  - openapi/apitube-fact-check-api-openapi.yml
  - openapi/apitube-news-api-openapi.yml
  - openapi/apitube-reference-api-openapi.yml
  - openapi/apitube-suggest-api-openapi.yml
  - openapi/apitube-system-api-openapi.yml
  - openapi/apitube-utilities-api-openapi.yml
  type: apiKey
- description: API key passed as a query parameter
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/apitube-account-api-openapi.yml
  - openapi/apitube-fact-check-api-openapi.yml
  - openapi/apitube-news-api-openapi.yml
  - openapi/apitube-reference-api-openapi.yml
  - openapi/apitube-suggest-api-openapi.yml
  - openapi/apitube-system-api-openapi.yml
  - openapi/apitube-utilities-api-openapi.yml
  type: apiKey
slug: apitube-authentication
source_filename: apitube-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://docs.apitube.io/platform/news-api/authentication.md (upgrading the profile derived from the seven refined OpenAPI documents)\ndocs: https://docs.apitube.io/platform/news-api/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  - bearer\nkey_model:\n  prefixes: {live: api_live_, test: api_test_}\n  bearer: 'The docs also accept the key as Authorization: Bearer <key> — a third passing style the specs do not declare.'\n  test_mode: Test keys hit the live API free of quota with body/body_html truncated; X-Apitube-Mode header reports live|test. See ../sandbox/apitube-sandbox.yml.\n  restrictions: Per-key endpoint scopes (403 ER0603 when missing), expiry dates (401 ER0230), IP allowlists (403 ER0601) and referrer/domain rules (403 ER0602), configured in the dashboard.\n  rotation: Keys can be regenerated from the dashboard if compromised.\n  errors: {missing: 401 ER0201, invalid: 401 ER0202,\
  \ expired: 401 ER0230}\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key passed as a request header\n  sources:\n  - openapi/apitube-account-api-openapi.yml\n  - openapi/apitube-fact-check-api-openapi.yml\n  - openapi/apitube-news-api-openapi.yml\n  - openapi/apitube-reference-api-openapi.yml\n  - openapi/apitube-suggest-api-openapi.yml\n  - openapi/apitube-system-api-openapi.yml\n  - openapi/apitube-utilities-api-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key passed as a query parameter\n  sources:\n  - openapi/apitube-account-api-openapi.yml\n  - openapi/apitube-fact-check-api-openapi.yml\n  - openapi/apitube-news-api-openapi.yml\n  - openapi/apitube-reference-api-openapi.yml\n  - openapi/apitube-suggest-api-openapi.yml\n  - openapi/apitube-system-api-openapi.yml\n  - openapi/apitube-utilities-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apitube/refs/heads/main/authentication/apitube-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- News
- Media Monitoring
- News API
- Fact Check
- Journalists
---
