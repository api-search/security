---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Appaegis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appaegis secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Appaegis
provider_slug: appaegis
scheme_count: 3
schemes:
- description: apiKey + apiSecret credential pair exchanged at /api/v2/authentication for an idToken. Created and revoked in the management portal.
  in: header
  name: apiKeySecret
  sources:
  - https://github.com/appaegis/api-script-samples/blob/main/lib/common.py
  type: apiKey
- description: Short-lived idToken presented on REST v1/v2 requests.
  in: header
  name: idTokenHeader
  parameter_name: idToken
  sources:
  - https://github.com/appaegis/api-script-samples/blob/main/lib/common.py
  type: apiKey
- bearer_format: JWT
  description: Same idToken presented as a Bearer token on the GraphQL endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - https://github.com/appaegis/api-script-samples/blob/main/block-list-pac-v2.py
  type: http
slug: appaegis-authentication
source_filename: appaegis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://github.com/appaegis/api-script-samples/blob/main/lib/common.py\ndocs: https://github.com/appaegis/api-script-samples#prerequisite\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  model: token-exchange\n  note: >-\n    No published OpenAPI/OIDC discovery document is available; this profile is\n    derived from the provider's public api-script-samples repository (lib/common.py)\n    and README, which document the real authentication flow verbatim.\nflow:\n  description: >-\n    Two-step token-exchange. An API key (apiKey) and secret (apiSecret) are issued\n    in the Mammoth Cyber management portal under \"Setting -> Admins & API Keys ->\n    API Keys\" (the secret is displayed once and can be downloaded as a dotenv file).\n    The client POSTs the apiKey/apiSecret pair to the authentication endpoint and\n    receives a short-lived idToken, which is then presented on subsequent calls.\n\
  \  token_exchange:\n    method: POST\n    url: https://api.mammothcyber.net/api/v2/authentication\n    request_content_type: application/json\n    request_body: '{ \"apiKey\": \"...\", \"apiSecret\": \"...\" }'\n    response_field: Authorization\n    returns: idToken (JWT)\n  presenting_the_token:\n    - surface: REST (v1 + v2)\n      header: idToken\n      value: <idToken>\n    - surface: GraphQL (/graphql, /api/graphql)\n      header: Authorization\n      value: Bearer <idToken>\nschemes:\n  - name: apiKeySecret\n    type: apiKey\n    in: header\n    description: >-\n      apiKey + apiSecret credential pair exchanged at /api/v2/authentication for an\n      idToken. Created and revoked in the management portal.\n    sources: [https://github.com/appaegis/api-script-samples/blob/main/lib/common.py]\n  - name: idTokenHeader\n    type: apiKey\n    in: header\n    parameter_name: idToken\n    description: Short-lived idToken presented on REST v1/v2 requests.\n    sources: [https://github.com/appaegis/api-script-samples/blob/main/lib/common.py]\n\
  \  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    description: Same idToken presented as a Bearer token on the GraphQL endpoint.\n    sources: [https://github.com/appaegis/api-script-samples/blob/main/block-list-pac-v2.py]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appaegis/refs/heads/main/authentication/appaegis-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Security
- Zero Trust
- Enterprise Browser
- Access Management
- Data Loss Prevention
- GenAI Security
- Identity
- SASE
---
