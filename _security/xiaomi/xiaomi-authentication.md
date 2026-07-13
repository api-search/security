---
api_key_in:
- header
api_specs:
- filename: xiaomi-open-api-openapi.yml
  format: yaml
  label: Xiaomi Open API
  slug: xiaomi-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-open-api-openapi.yml
- filename: xiaomi-galaxy-fds-openapi.yml
  format: yaml
  label: Xiaomi Galaxy FDS API
  slug: xiaomi-galaxy-fds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-galaxy-fds-openapi.yml
- filename: xiaomi-mimo-api-openapi.yml
  format: yaml
  label: Xiaomi MiMo AI API
  slug: xiaomi-mimo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-mimo-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Xiaomi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Xiaomi secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Xiaomi
provider_slug: xiaomi
scheme_count: 3
schemes:
- description: HMAC-based signature authentication. Requests must include a Date header and Authorization header with HMAC-SHA1 signature.
  name: hmacAuth
  scheme: custom
  sources:
  - openapi/xiaomi-galaxy-fds-openapi.yml
  type: http
- description: API key obtained from the Xiaomi MiMo console.
  in: header
  name: apiKeyAuth
  parameter: api-key
  sources:
  - openapi/xiaomi-mimo-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://account.xiaomi.com/oauth2/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://account.xiaomi.com/oauth2/token
  name: oauth2
  sources:
  - openapi/xiaomi-open-api-openapi.yml
  type: oauth2
slug: xiaomi-authentication
source_filename: xiaomi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xiaomi-galaxy-fds-openapi.yml, openapi/xiaomi-mimo-api-openapi.yml, openapi/xiaomi-open-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: hmacAuth\n  type: http\n  scheme: custom\n  description: HMAC-based signature authentication. Requests must include a Date header and\n    Authorization header with HMAC-SHA1 signature.\n  sources:\n  - openapi/xiaomi-galaxy-fds-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: API key obtained from the Xiaomi MiMo console.\n  sources:\n  - openapi/xiaomi-mimo-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.xiaomi.com/oauth2/authorize\n    tokenUrl: https://account.xiaomi.com/oauth2/token\n    scopes: 5\n  sources:\n  - openapi/xiaomi-open-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/authentication/xiaomi-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Consumer Electronics
- IoT
- Smart Home
- Mobile
- Artificial Intelligence
- Cloud Storage
- Machine Learning
---
