---
api_key_in:
- query
auth_types:
- access_token
description: Xiaoe Open API authentication. Applications are created and authorized in the Xiaoe cloud console, then exchange app credentials for a short-lived access_token that is passed on every subsequent API call. There is no OAuth2 authorization-code / scope model — permissions are granted per-interface in the console and enforced server-side (return code 2017 on missing permission), with optional IP whitelisting (return code 2051).
kind: authentication
layout: security
method: searched
name: Sem Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xiaoe (小鹅通) secures its APIs with access_token across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Xiaoe (小鹅通)
provider_slug: sem
scheme_count: 0
schemes: []
slug: sem-authentication
source_filename: sem-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api-doc.xiaoe-tech.com/develop_guide/get_access_token.html\ndescription: >-\n  Xiaoe Open API authentication. Applications are created and authorized in the\n  Xiaoe cloud console, then exchange app credentials for a short-lived\n  access_token that is passed on every subsequent API call. There is no OAuth2\n  authorization-code / scope model — permissions are granted per-interface in\n  the console and enforced server-side (return code 2017 on missing permission),\n  with optional IP whitelisting (return code 2051).\nsummary:\n  types: [access_token]\n  token_endpoint: https://api.xiaoe-tech.com/token\n  oauth2_flows: []\n  api_key_in: [query]\ntoken:\n  endpoint: GET https://api.xiaoe-tech.com/token\n  params:\n    app_id: Store business identifier\n    client_id: Application unique identifier\n    secret_key: Application credential secret\n    grant_type: Fixed value client_credential\n  grant_type: client_credential\n\
  \  ttl_seconds: 7200\n  refresh: >-\n    Requests with >30 min remaining return the same token; below 30 min a new\n    token is issued while the old remains briefly valid. Token endpoint is rate\n    limited to 100 requests per 10 minutes.\n  response_fields: [access_token, expires_in]\npermissions:\n  model: per-interface authorization granted in the Xiaoe cloud console\n  ip_whitelist: supported (return code 2051 when caller IP is not whitelisted)\ndocs: https://api-doc.xiaoe-tech.com/develop_guide/get_access_token.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sem/refs/heads/main/authentication/sem-authentication.yml
summary_line: access_token · 0 schemes
tags:
- Company
- SaaS
- Private Domain
- Content Commerce
- Live Streaming
- Education
- E-Commerce
- Marketing
- WeChat
- China
---
