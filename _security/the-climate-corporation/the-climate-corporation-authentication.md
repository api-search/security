---
api_key_in:
- header
api_specs:
- filename: the-climate-corporation-platform-openapi-original.yml
  format: yaml
  label: Climate FieldView Platform API
  slug: climate-fieldview-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-climate-corporation/refs/heads/main/openapi/the-climate-corporation-platform-openapi-original.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: The Climate Corporation Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: The Climate Corporation secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: The Climate Corporation
provider_slug: the-climate-corporation
scheme_count: 2
schemes:
- description: 'Log in with FieldView OAuth2 provider (Authorization Code Grant). Used to authorize the client (partner) and

    user. The *access_token* is required to be provided in the `Authorization` header on all calls to the FieldView

    APIs with the following format `Bearer $access_token`.'
  flows:
  - authorizationUrl: https://climate.com/static/app-login/
    flow: authorizationCode
    scopes: 21
    tokenUrl: https://api.climate.com/api/oauth/token
  name: oauth2_authorization_code
  sources:
  - openapi/the-climate-corporation-platform-openapi-original.yml
  type: oauth2
- description: 'API access key used to control throttling (429 responses).  This key is typically formatted:

    `partner-{name}-{uuid}`'
  in: header
  name: api_key
  parameter: X-Api-Key
  sources:
  - openapi/the-climate-corporation-platform-openapi-original.yml
  type: apiKey
slug: the-climate-corporation-authentication
source_filename: the-climate-corporation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  openapi/the-climate-corporation-platform-openapi-original.yml (v4.0.11),\n  upgraded from the FieldView OAuth2 Overview at\n  https://dev.fieldview.com/api-details/\ndocs: https://dev.fieldview.com/api-details/\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  required_together: >-\n    Every call requires BOTH a Bearer access_token (OAuth2) AND the X-Api-Key\n    header. Missing token -> 401 {\"message\":\"Unauthorized\"}; missing/invalid\n    X-Api-Key -> 403 {\"message\":\"Forbidden\"}.\n  token_endpoint_auth: HTTP Basic base64(clientId:clientSecret) on POST https://api.climate.com/api/oauth/token\n  grants: [authorization_code, refresh_token]\n  access_token_ttl: 4 hours\n  refresh_token_ttl: 30 days (single-use)\n  tls: TLS 1.2, HTTPS only\nschemes:\n- name: oauth2_authorization_code\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://climate.com/static/app-login/\n    tokenUrl: https://api.climate.com/api/oauth/token\n    scopes: 21\n  description: |-\n    Log in with FieldView OAuth2 provider (Authorization Code Grant). Used to authorize the client (partner) and\n    user. The *access_token* is required to be provided in the `Authorization` header on all calls to the FieldView\n    APIs with the following format `Bearer $access_token`.\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: |-\n    API access key used to control throttling (429 responses).  This key is typically formatted:\n    `partner-{name}-{uuid}`\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-climate-corporation/refs/heads/main/authentication/the-climate-corporation-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Climate
- Agriculture
- AgTech
- Digital Agriculture
- Farm Management
- Geospatial
- APIs
---
