---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Didi Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Didi secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Didi
provider_slug: didi
scheme_count: 1
schemes:
- base_url: https://api.es.xiaojukeji.com
  credentials:
    client_id: required (clientId — client identity)
    client_secret: required (clientSecret — client secret)
    sign_key: required (signKey — request signing key, separate from client_secret)
  flow: clientCredentials
  grant_type: client_credentials
  ip_allow_list: required (IP whitelist configured per application)
  name: DDESClientCredentials
  payload_encryption:
    supported: true
    type: AES128/AES256 (optional whole-payload AES, default off)
  signing:
    default: MD5
    methods:
    - MD5
    - SHA256
    required: true
  sources:
  - https://github.com/didi/ddes-openapi-sdk-java
  - https://opendocs.xiaojukeji.com/version2024
  token:
    auto_managed: true
    grant_type: client_credentials
    retry_on_unauthorized: default 2 retries, 1000ms interval
  type: oauth2
slug: didi-authentication
source_filename: didi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  DiDi Enterprise Services (DDES) Open API access guide\n  https://opendocs.xiaojukeji.com/version2024 (接入前必读 /version2024/10957) and the\n  official Java SDK config reference\n  https://github.com/didi/ddes-openapi-sdk-java (com.xiaoju.open.sdk.didies.core.Config).\n  Derived from published SDK defaults and the docs onboarding flow; no OpenAPI\n  securitySchemes are published for this API.\ndocs: https://opendocs.xiaojukeji.com/version2024\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  request_signing: true\n  notes: >-\n    App-level (machine-to-machine) authentication. There is no per-user OAuth\n    scope surface; access is governed by the enterprise application plus an IP\n    allow-list, so no scopes/ artifact is emitted.\nschemes:\n  - name: DDESClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    grant_type: client_credentials\n    base_url: https://api.es.xiaojukeji.com\n\
  \    credentials:\n      client_id: required (clientId — client identity)\n      client_secret: required (clientSecret — client secret)\n      sign_key: required (signKey — request signing key, separate from client_secret)\n    token:\n      grant_type: client_credentials\n      auto_managed: true\n      retry_on_unauthorized: default 2 retries, 1000ms interval\n    signing:\n      required: true\n      methods: [MD5, SHA256]\n      default: MD5\n    payload_encryption:\n      supported: true\n      type: AES128/AES256 (optional whole-payload AES, default off)\n    ip_allow_list: required (IP whitelist configured per application)\n    sources:\n      - https://github.com/didi/ddes-openapi-sdk-java\n      - https://opendocs.xiaojukeji.com/version2024\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/didi/refs/heads/main/authentication/didi-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Mobility
- Ride Hailing
- Transportation
- Enterprise Travel
- Expense Management
- OAuth
---
