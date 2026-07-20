---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Appneta Broadcom Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppNeta (Broadcom Software) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AppNeta (Broadcom Software)
provider_slug: appneta-broadcom-software
scheme_count: 1
schemes:
- description: 'API access token credential. Pass as: Authorization: Token <token>. Applies to both the v3 (Classic) and v4 (Intelligent Alarms) APIs.'
  example: "curl -X GET \\\n  -H \"Authorization: Token <token>\" \\\n  -H \"Accept: application/json\" \\\n  \"https://<application_cluster>.pm.appneta.com/api/v4/networkPath\"\n"
  in: header
  name: ApiAccessToken
  parameter: Authorization
  scheme_prefix: Token
  sources:
  - docs
  type: apiKey
slug: appneta-broadcom-software-authentication
source_filename: appneta-broadcom-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://techdocs.broadcom.com/us/en/ca-enterprise-software/it-operations-management/appneta/GA/integrate/api/api-access-tokens.html\ndocs: https://techdocs.broadcom.com/us/en/ca-enterprise-software/it-operations-management/appneta/GA/integrate/api-access-tokens.html\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    AppNeta authenticates REST API requests with an API access token passed in the\n    HTTP Authorization header using the \"Token\" scheme. Tokens are created in the\n    AppNeta web app and can be granted specific scope and permission levels without\n    creating additional AppNeta users. There is no OAuth 2.0 authorization-code flow;\n    the token is a long-lived bearer-style credential.\nschemes:\n  - name: ApiAccessToken\n    type: apiKey\n    in: header\n    parameter: Authorization\n    scheme_prefix: \"Token\"\n    description: >-\n      API access token credential.\
  \ Pass as: Authorization: Token <token>. Applies to\n      both the v3 (Classic) and v4 (Intelligent Alarms) APIs.\n    example: |\n      curl -X GET \\\n        -H \"Authorization: Token <token>\" \\\n        -H \"Accept: application/json\" \\\n        \"https://<application_cluster>.pm.appneta.com/api/v4/networkPath\"\n    sources: [docs]\ntoken_management:\n  creation: AppNeta web application (Manage > API Access Tokens)\n  scoped: true\n  scope_note: >-\n    Tokens can be issued with varying scope and permission levels to constrain what a\n    given script or integration may access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appneta-broadcom-software/refs/heads/main/authentication/appneta-broadcom-software-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Network Monitoring
- Network Performance
- Observability
- Application Performance
- Digital Experience Monitoring
- Synthetic Monitoring
- IT Operations
- Broadcom
- Ai Infrastructure
---
