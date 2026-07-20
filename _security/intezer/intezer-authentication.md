---
api_key_in:
- body
auth_types:
- apiKey
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Intezer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Intezer secures its APIs with apiKey and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Intezer
provider_slug: intezer
scheme_count: 2
schemes:
- description: Clients POST their API key to /api/v2-0/get-access-token to obtain a short-lived JWT. The API key is generated in the Intezer Analyze account page (Account > API Access > Generate API Key) and can be supplied via the INTEZER_ANALYZE_API_KEY environment variable to the SDK/CLI.
  in: body
  name: ApiKeyAccessToken
  token_endpoint: https://analyze.intezer.com/api/v2-0/get-access-token
  type: apiKey
- bearerFormat: JWT
  description: 'The access token returned by get-access-token is sent as `Authorization: Bearer <jwt>` on every subsequent API request.'
  name: BearerJWT
  scheme: bearer
  type: http
slug: intezer-authentication
source_filename: intezer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/intezer/analyze-python-sdk/blob/master/intezer_sdk/api.py ; https://docs.intezer.com/docs\ndocs: https://docs.intezer.com/docs\nsummary:\n  types: [apiKey, http-bearer]\n  api_key_in: [body]\n  bearer_source: access-token-exchange\nschemes:\n  - name: ApiKeyAccessToken\n    type: apiKey\n    in: body\n    description: >-\n      Clients POST their API key to /api/v2-0/get-access-token to obtain a short-lived\n      JWT. The API key is generated in the Intezer Analyze account page (Account >\n      API Access > Generate API Key) and can be supplied via the INTEZER_ANALYZE_API_KEY\n      environment variable to the SDK/CLI.\n    token_endpoint: https://analyze.intezer.com/api/v2-0/get-access-token\n  - name: BearerJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      The access token returned by get-access-token is sent as\n      `Authorization: Bearer <jwt>` on every subsequent\
  \ API request.\nnotes: >-\n  Derived from the official Python SDK auth flow and confirmed against the public docs\n  landing. Full API reference (docs.intezer.com/docs) is access-gated. On-premise\n  deployments accept a custom base URL (http://<address>/api).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intezer/refs/heads/main/authentication/intezer-authentication.yml
summary_line: apiKey/http-bearer · 2 schemes
tags:
- Company
- Cybersecurity
- Security
- Malware Analysis
- Threat Intelligence
- SOC
- Incident Response
- Artificial Intelligence
- Automation
---
