---
api_key_in: []
api_specs:
- filename: coviu-rest-api-openapi.json
  format: json
  label: Coviu Sessions API
  slug: coviu-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-rest-api-openapi.json
- filename: coviu-rest-api-openapi.json
  format: json
  label: Coviu Participants API
  slug: coviu-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-rest-api-openapi.json
- filename: coviu-rest-api-openapi.json
  format: json
  label: Coviu Waiting Area API
  slug: coviu-waiting-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-rest-api-openapi.json
- filename: coviu-rest-api-openapi.json
  format: json
  label: Coviu Collections API
  slug: coviu-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-rest-api-openapi.json
- filename: coviu-rest-api-openapi.json
  format: json
  label: Coviu Webhooks
  slug: coviu-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-rest-api-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Coviu Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- refreshToken
overview: Coviu secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, and refreshToken flow(s).
provider_name: Coviu
provider_slug: coviu
scheme_count: 2
schemes:
- description: Used to request an access token. Supply the Client ID and Client Secret as the username and password.
  name: Basic
  scheme: basic
  sources:
  - openapi/coviu-rest-api-openapi.json
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /v1/auth/token
  - flow: authorizationCode
    source: https://coviu.readme.io/reference/access-token
    tokenUrl: /v1/auth/token
  - flow: refreshToken
    source: https://coviu.readme.io/reference/access-token
    tokenUrl: /v1/auth/token
  name: ClientCredentials
  sources:
  - openapi/coviu-rest-api-openapi.json
  - https://coviu.readme.io/reference/access-token
  type: oauth2
slug: coviu-authentication
source_filename: coviu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/coviu-rest-api-openapi.json\ndocs: https://coviu.readme.io/reference/access-token\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  - refreshToken\nnotes: >-\n  The Coviu access-token reference (coviu.readme.io/reference/access-token) documents three OAuth2\n  grant types at POST /v1/auth/token — client_credentials, authorization_code, and refresh_token —\n  all authenticated with HTTP Basic (Client ID as username, Client Secret as password) and an\n  application/x-www-form-urlencoded body. The harvested OpenAPI only declares the clientCredentials\n  flow, so the authorizationCode and refreshToken flows are sourced from the docs.\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  description: Used to request an access token. Supply the Client ID and Client Secret as the\n    username and password.\n  sources:\n  - openapi/coviu-rest-api-openapi.json\n\
  - name: ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/auth/token\n    scopes: 0\n  - flow: authorizationCode\n    tokenUrl: /v1/auth/token\n    source: https://coviu.readme.io/reference/access-token\n  - flow: refreshToken\n    tokenUrl: /v1/auth/token\n    source: https://coviu.readme.io/reference/access-token\n  sources:\n  - openapi/coviu-rest-api-openapi.json\n  - https://coviu.readme.io/reference/access-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/authentication/coviu-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Healthcare
- Telehealth
- Australia
- Virtual Care
- Video
- WebRTC
- Appointments
- Remote Monitoring
- REST
---
