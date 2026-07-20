---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Appneta Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppNeta secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AppNeta
provider_slug: appneta
scheme_count: 1
schemes:
- description: 'AppNeta API requests are authenticated with an API access token passed in the Authorization request header with the literal scheme word "Token", e.g. `Authorization: Token <token>`. Token values are case sensitive. Tokens are created and managed in AppNeta Performance Manager (API Access Tokens admin); they let scripts and applications call the API without embedding a username and password.'
  example_request: 'curl -X GET -H "Authorization: Token <token>" -H "Accept: application/json" "https://<node>.pm.appneta.com/api/v3/path"'
  header_name: Authorization
  in: header
  name: ApiAccessToken
  sources:
  - docs
  type: apiKey
  value_format: Token <api_access_token>
slug: appneta-authentication
source_filename: appneta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://techdocs.broadcom.com/us/en/ca-enterprise-software/it-operations-management/appneta/GA/integrate/api-access-tokens.html\ndocs: https://techdocs.broadcom.com/us/en/ca-enterprise-software/it-operations-management/appneta/GA/integrate/api-access-tokens.html\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: ApiAccessToken\n  type: apiKey\n  in: header\n  header_name: Authorization\n  value_format: Token <api_access_token>\n  description: >-\n    AppNeta API requests are authenticated with an API access token passed in the\n    Authorization request header with the literal scheme word \"Token\", e.g.\n    `Authorization: Token <token>`. Token values are case sensitive. Tokens are\n    created and managed in AppNeta Performance Manager (API Access Tokens admin);\n    they let scripts and applications call the API without embedding a username and\n    password.\n  example_request:\
  \ >-\n    curl -X GET -H \"Authorization: Token <token>\" -H \"Accept: application/json\"\n    \"https://<node>.pm.appneta.com/api/v3/path\"\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appneta/refs/heads/main/authentication/appneta-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Network Monitoring
- Network Performance Monitoring
- Observability
- Application Performance Monitoring
- Synthetic Monitoring
- Monitoring
- Broadcom
---
