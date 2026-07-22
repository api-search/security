---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Parallels Swsoft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parallels (SWSoft) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parallels (SWSoft)
provider_slug: parallels-swsoft
scheme_count: 1
schemes:
- in: header
  name: session_token
  obtained_via:
    operation: POST api/session/logon
    request_body: '{ "username": "...", "password": "..." }'
    response_field: authToken
  parameter: auth_token
  scheme: token
  sources:
  - docs.parallels.com/landing/ras-rest-api-guide
  type: http
slug: parallels-swsoft-authentication
source_filename: parallels-swsoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.parallels.com/landing/ras-rest-api-guide\ndocs: https://docs.parallels.com/landing/ras-rest-api-guide/examples/basic-sample\nsummary:\n  types: [http]\n  scheme: token\n  note: >-\n    Parallels RAS REST API uses a custom session-token scheme. The client logs\n    on with administrator credentials and receives an authToken, which is then\n    supplied on every subsequent request via the auth_token request header. The\n    API is served by the self-hosted RAS server (default TCP port 20443), so the\n    token is issued and validated by the customer's own RAS deployment, not by a\n    Parallels-hosted identity provider. There is no OAuth2/OIDC on the REST API.\nschemes:\n  - name: session_token\n    type: http\n    scheme: token\n    in: header\n    parameter: auth_token\n    obtained_via:\n      operation: POST api/session/logon\n      request_body: '{ \"username\": \"...\", \"password\": \"...\" }'\n      response_field:\
  \ authToken\n    sources: [docs.parallels.com/landing/ras-rest-api-guide]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallels-swsoft/refs/heads/main/authentication/parallels-swsoft-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Virtualization
- Remote Desktop
- Application Delivery
- Cloud Infrastructure
- VDI
- Automation
- REST API
---
