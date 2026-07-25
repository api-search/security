---
api_key_in: []
api_specs:
- filename: databento-timeseries-api-openapi.yml
  format: yaml
  label: Databento Historical Timeseries API
  slug: databento-historical-timeseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-timeseries-api-openapi.yml
- filename: databento-metadata-api-openapi.yml
  format: yaml
  label: Databento Metadata API
  slug: databento-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-metadata-api-openapi.yml
- filename: databento-symbology-api-openapi.yml
  format: yaml
  label: Databento Symbology API
  slug: databento-symbology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-symbology-api-openapi.yml
- filename: databento-batch-api-openapi.yml
  format: yaml
  label: Databento Batch API
  slug: databento-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-batch-api-openapi.yml
- filename: databento-reference-api-openapi.yml
  format: yaml
  label: Databento Reference API
  slug: databento-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-reference-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Databento Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Databento secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Databento
provider_slug: databento
scheme_count: 2
schemes:
- description: HTTP Basic authentication. Supply your Databento API key (prefixed with db-) as the username and leave the password empty.
  name: apiKeyBasicAuth
  scheme: basic
  sources:
  - openapi/databento-batch-api-openapi.yml
  - openapi/databento-metadata-api-openapi.yml
  - openapi/databento-platform-openapi-official.json
  - openapi/databento-reference-api-openapi.yml
  - openapi/databento-symbology-api-openapi.yml
  - openapi/databento-timeseries-api-openapi.yml
  type: http
- flows:
  - flow: password
    scopes: 0
    tokenUrl: /v0/auth/login
  name: OAuth2PasswordBearerWithCookie
  sources:
  - openapi/databento-platform-openapi-official.json
  type: oauth2
slug: databento-authentication
source_filename: databento-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: openapi/databento-batch-api-openapi.yml, openapi/databento-metadata-api-openapi.yml,\n  openapi/databento-platform-openapi-official.json, openapi/databento-reference-api-openapi.yml,\n  openapi/databento-symbology-api-openapi.yml, openapi/databento-timeseries-api-openapi.yml\ndocs: https://databento.com/docs/api-reference-historical/basics/authentication\nnotes: >-\n  All HTTP (historical/reference) requests authenticate with HTTP Basic: the\n  Databento API key (32 characters, prefixed db-) is the username and the\n  password is left empty. API keys are created and rotated in the user portal.\n  The Live Streaming API (raw TCP, DBN protocol) does not use HTTP Basic;\n  sessions authenticate with a CRAM challenge-response handshake using the same\n  API key (docs: https://databento.com/docs/api-reference-live/basics/authentication).\n  The OAuth2 password flow below (tokenUrl /v0/auth/login) is the portal's own\n  cookie/session\
  \ login exposed in the platform OpenAPI, not a public OAuth\n  surface for API consumers - it defines no scopes.\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: apiKeyBasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Supply your Databento API key (prefixed with db-)\n    as the username and leave the password empty.\n  sources:\n  - openapi/databento-batch-api-openapi.yml\n  - openapi/databento-metadata-api-openapi.yml\n  - openapi/databento-platform-openapi-official.json\n  - openapi/databento-reference-api-openapi.yml\n  - openapi/databento-symbology-api-openapi.yml\n  - openapi/databento-timeseries-api-openapi.yml\n- name: OAuth2PasswordBearerWithCookie\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /v0/auth/login\n    scopes: 0\n  sources:\n  - openapi/databento-platform-openapi-official.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/authentication/databento-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Market Data
- Financial Data
- Reference Data
- Historical Market Data
- Trading
---
