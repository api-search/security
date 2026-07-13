---
api_key_in: []
api_specs:
- filename: quodd-openapi.yml
  format: yaml
  label: QUODD Snap API
  slug: quodd-snap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/openapi/quodd-openapi.yml
- filename: quodd-openapi.yml
  format: yaml
  label: QUODD Batch Snaps API
  slug: quodd-batch-snaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/openapi/quodd-openapi.yml
- filename: quodd-openapi.yml
  format: yaml
  label: QUODD Options Snaps API
  slug: quodd-options-snaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/openapi/quodd-openapi.yml
- filename: quodd-openapi.yml
  format: yaml
  label: QUODD Authentication Token API
  slug: quodd-authentication-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/openapi/quodd-openapi.yml
- filename: quodd-openapi.yml
  format: yaml
  label: QUODD Ticker Search API
  slug: quodd-ticker-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/openapi/quodd-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Quodd Authentication
name_suffix: Authentication
oauth_flows: []
overview: QUODD secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: QUODD
provider_slug: quodd
scheme_count: 1
schemes:
- description: QUODD uses token-based authentication. Trial or firm users exchange a username and password for an access token via the token endpoints (POST token-for-trial-user / token-for-firm-user). The token is appended to each REST request as the `_token` query parameter and expires after 24 hours, after which a new token must be generated. Production credentials are provisioned through a trial or an enterprise agreement with QUODD.
  in: query
  keyName: _token
  name: tokenQuery
  sources:
  - https://developer.quodd.com/docs/rest-api/post-token-for-trial-user
  - https://developer.quodd.com/docs/rest-api/post-token-for-firm-user
  - https://www.quodd.com/faqs/what-is-an-api-token
  type: apiKey
slug: quodd-authentication
source_filename: quodd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quodd-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: tokenQuery\n  type: apiKey\n  in: query\n  keyName: _token\n  description: >-\n    QUODD uses token-based authentication. Trial or firm users exchange a\n    username and password for an access token via the token endpoints (POST\n    token-for-trial-user / token-for-firm-user). The token is appended to each\n    REST request as the `_token` query parameter and expires after 24 hours,\n    after which a new token must be generated. Production credentials are\n    provisioned through a trial or an enterprise agreement with QUODD.\n  sources:\n  - https://developer.quodd.com/docs/rest-api/post-token-for-trial-user\n  - https://developer.quodd.com/docs/rest-api/post-token-for-firm-user\n  - https://www.quodd.com/faqs/what-is-an-api-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/authentication/quodd-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Market Data
- Real-Time Data
- Financial Data
- Streaming
- Historical Data
- Reference Data
- Quotes
- Fintech
---
