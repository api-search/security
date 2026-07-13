---
api_key_in:
- query
api_specs:
- filename: bitrix24-openapi.json
  format: json
  label: Bitrix24 REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrix24/refs/heads/main/openapi/bitrix24-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bitrix24 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Bitrix24 secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Bitrix24
provider_slug: bitrix24
scheme_count: 2
schemes:
- description: OAuth 2.0 access_token or incoming webhook token
  in: query
  name: AccessToken
  parameter: auth
  sources:
  - openapi/bitrix24-openapi.json
  type: apiKey
- description: OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://oauth.bitrix.info/oauth/authorize/
    flow: authorizationCode
    scopes: 45
    tokenUrl: https://oauth.bitrix.info/oauth/token/
  name: OAuth2
  sources:
  - openapi/bitrix24-openapi.json
  type: oauth2
slug: bitrix24-authentication
source_filename: bitrix24-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bitrix24-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: query\n  parameter: auth\n  description: OAuth 2.0 access_token or incoming webhook token\n  sources:\n  - openapi/bitrix24-openapi.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.bitrix.info/oauth/authorize/\n    tokenUrl: https://oauth.bitrix.info/oauth/token/\n    scopes: 45\n  description: OAuth 2.0 authorization\n  sources:\n  - openapi/bitrix24-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitrix24/refs/heads/main/authentication/bitrix24-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- CRM
- Collaboration
- Project Management
- Tasks
- Telephony
- Contact Center
- Document Management
- HR
- Business Suite
---
