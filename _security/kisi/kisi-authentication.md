---
api_key_in:
- header
api_specs:
- filename: kisi-openapi-original.yml
  format: yaml
  label: Kisi API
  slug: kisi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kisi/refs/heads/main/openapi/kisi-openapi-original.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Kisi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: KISI secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: KISI
provider_slug: kisi
scheme_count: 4
schemes:
- description: 'Authorize using a signature of the request body. The signature is a HMAC-SHA256 hash of the request body using a secret key. <br><br>E.g. `X-Signature: 123`'
  in: header
  name: Webhook-Signature
  parameter: X-Signature
  sources:
  - openapi/kisi-openapi-original.yml
  type: apiKey
- description: 'Authorize using a login. Prefix the value with `KISI-LOGIN`<br><br>Example: `Authorization: KISI-LOGIN 123`'
  in: header
  name: Kisi-Login
  parameter: Authorization
  sources:
  - openapi/kisi-openapi-original.yml
  type: apiKey
- description: Username is the client id. Password is the client secret.
  name: OAuth2Basic
  scheme: basic
  sources:
  - openapi/kisi-openapi-original.yml
  type: http
- description: 'OAuth access tokens are sent as bearer tokens. Example: `Authorization: Bearer youraccesstoken`'
  flows:
  - authorizationUrl: https://api.kisi.io/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.kisi.io/oauth/token
  name: OAuth2
  sources:
  - openapi/kisi-openapi-original.yml
  type: oauth2
slug: kisi-authentication
source_filename: kisi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/kisi-openapi-original.yml\ndocs: https://docs.kisi.io/api/get_started/add_necessary_headers\nnote: >-\n  Header-based auth on the Authorization header. Four apiKey variants share the\n  Authorization header (Kisi-Login, Kisi-Access-Key, Kisi-Group-Link, Kisi-Service),\n  distinguished by value prefix; OAuth2 authorizationCode issues bearer tokens.\n  Webhook-Signature (X-Signature, HMAC-SHA256) verifies inbound webhook payloads.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: Webhook-Signature\n  type: apiKey\n  in: header\n  parameter: X-Signature\n  description: 'Authorize using a signature of the request body. The signature is a HMAC-SHA256\n    hash of the request body using a secret key. <br><br>E.g. `X-Signature: 123`'\n  sources:\n  - openapi/kisi-openapi-original.yml\n- name: Kisi-Login\n  type: apiKey\n  in: header\n\
  \  parameter: Authorization\n  description: 'Authorize using a login. Prefix the value with `KISI-LOGIN`<br><br>Example:\n    `Authorization: KISI-LOGIN 123`'\n  sources:\n  - openapi/kisi-openapi-original.yml\n- name: OAuth2Basic\n  type: http\n  scheme: basic\n  description: Username is the client id. Password is the client secret.\n  sources:\n  - openapi/kisi-openapi-original.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.kisi.io/oauth/authorize\n    tokenUrl: https://api.kisi.io/oauth/token\n    scopes: 0\n  description: 'OAuth access tokens are sent as bearer tokens. Example: `Authorization: Bearer\n    youraccesstoken`'\n  sources:\n  - openapi/kisi-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kisi/refs/heads/main/authentication/kisi-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- Physical Access Control
- Security
- Identity
- IoT
- Building Management
- Access Control
- SaaS
---
