---
api_key_in: []
api_specs:
- filename: indico-data-openapi.yml
  format: yaml
  label: Indico REST API
  slug: indico-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indico-data/refs/heads/main/openapi/indico-data-openapi.yml
auth_types:
- http-basic
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Indico Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Indico Data secures its APIs with http-basic and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Indico Data
provider_slug: indico-data
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/indico-data-openapi.yml
  type: http
  used_for: /api/v1/auth/refreshToken (token exchange only)
- bearer_format: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/indico-data-openapi.yml
  token_lifetime: 15 minutes
  type: http
  used_for: all data endpoints
slug: indico-data-authentication
source_filename: indico-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.indicodata.ai/docs/getting-started\ndocs: https://developer.indicodata.ai/docs/getting-started\nsummary:\n  types: [http-basic, http-bearer]\n  api_key_in: []\n  oauth2_flows: []\n  model: >-\n    Two-step token auth. Download an API token from the Account page of the\n    Intake / Agent Studio app. POST it via HTTP Basic Authentication to\n    /restapi/api/v1/auth/refreshToken to receive a short-lived JWT access_token\n    (expires after 15 minutes). Send that JWT as a Bearer token on all other REST\n    endpoints. Generating a new API token immediately expires all prior tokens.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    used_for: /api/v1/auth/refreshToken (token exchange only)\n    sources: [openapi/indico-data-openapi.yml]\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    token_lifetime: 15 minutes\n    used_for: all data endpoints\n    sources:\
  \ [openapi/indico-data-openapi.yml]\nnotes:\n  - The GraphQL API (served at /graph/api/graphql) uses the same JWT bearer token.\n  - No OAuth2 authorization/scope surface is documented; there are no OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indico-data/refs/heads/main/authentication/indico-data-authentication.yml
summary_line: http-basic/http-bearer · 2 schemes
tags:
- Company
- Intelligent Document Processing
- Intelligent Process Automation
- Document AI
- Machine Learning
- Unstructured Data
- Data Extraction
- Insurance
---
