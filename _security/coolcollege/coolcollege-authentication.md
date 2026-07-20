---
api_key_in:
- query
api_specs:
- filename: coolcollege-openapi-original.json
  format: json
  label: 酷学院 REST API (Cool College Open API)
  slug: 酷学院-rest-api-cool-college-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolcollege/refs/heads/main/openapi/coolcollege-openapi-original.json
auth_types:
- signature
- token
description: ''
kind: authentication
layout: security
method: searched
name: Coolcollege Authentication
name_suffix: Authentication
oauth_flows: []
overview: 酷学院 (Cool College) secures its APIs with signature and token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 酷学院 (Cool College)
provider_slug: coolcollege
scheme_count: 1
schemes:
- credentials:
  - description: apiKey issued to the enterprise in the open platform console.
    in: query
    name: api_key
  - description: apiSecret (signing key).
    in: query
    name: api_secret
  - description: 13-digit millisecond timestamp.
    in: query
    name: timestamp
  - algorithm: HmacSHA256
    description: HmacSHA256 over the string (timestamp + "\n" + apiKey) keyed by apiSecret, then URL-encoded before being appended to the request URL.
    in: query
    name: signature
  exchange_operation: openapi/coolcollege-openapi-original.json#GET /{enterprise-id}/get_access_token
  name: hmac-signature-exchange
  returns:
    note: get_access_token returns an access_token used to authorize subsequent API calls. The spec does not declare how the access_token is transmitted on downstream requests; consult https://open.coolcollege.cn/ for the header/param binding.
    token: access_token
  tenant_scope: Every operation is scoped to a tenant via the {enterprise-id} path parameter.
  type: signature
slug: coolcollege-authentication
source_filename: coolcollege-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/coolcollege-openapi-original.json\ndocs: https://open.coolcollege.cn/\nsummary:\n  types: [signature, token]\n  api_key_in: [query]\n  oauth2_flows: []\nnote: >-\n  The 酷学院 (Cool College) Open API uses an HMAC-signature credential exchange rather than\n  OAuth2. The OpenAPI declares no components.securitySchemes; the model below is captured\n  from the get_access_token operation and its parameter descriptions.\nschemes:\n  - name: hmac-signature-exchange\n    type: signature\n    exchange_operation: 'openapi/coolcollege-openapi-original.json#GET /{enterprise-id}/get_access_token'\n    credentials:\n      - name: api_key\n        in: query\n        description: apiKey issued to the enterprise in the open platform console.\n      - name: api_secret\n        in: query\n        description: apiSecret (signing key).\n      - name: timestamp\n        in: query\n        description: 13-digit millisecond timestamp.\n      -\
  \ name: signature\n        in: query\n        algorithm: HmacSHA256\n        description: >-\n          HmacSHA256 over the string (timestamp + \"\\n\" + apiKey) keyed by apiSecret, then\n          URL-encoded before being appended to the request URL.\n    returns:\n      token: access_token\n      note: >-\n        get_access_token returns an access_token used to authorize subsequent API calls. The\n        spec does not declare how the access_token is transmitted on downstream requests;\n        consult https://open.coolcollege.cn/ for the header/param binding.\n    tenant_scope: 'Every operation is scoped to a tenant via the {enterprise-id} path parameter.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coolcollege/refs/heads/main/authentication/coolcollege-authentication.yml
summary_line: signature/token · 1 scheme
tags:
- Company
- Corporate Training
- E-Learning
- Talent Development
- Human Resources
- SaaS
- Learning Management
- China
---
