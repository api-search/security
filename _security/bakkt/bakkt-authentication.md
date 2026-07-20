---
api_key_in:
- header
api_specs:
- filename: bakkt-crypto-openapi.yml
  format: yaml
  label: Bakkt Crypto Solutions API
  slug: bakkt-crypto-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-crypto-openapi.yml
auth_types:
- http-token
description: ''
kind: authentication
layout: security
method: searched
name: Bakkt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bakkt secures its APIs with http-token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bakkt
provider_slug: bakkt
scheme_count: 1
schemes:
- description: Clients call POST /apex-crypto/api/v2/login (Crypto Solutions) or Generate Access Token (Fiat/Partner) with a provisioned logonId/password to obtain a short-lived security token, then pass it in the Authorization header on every subsequent request over HTTPS.
  header: Authorization
  in: header
  name: BakktSecurityToken
  obtain_operations:
  - login
  - generateAccessToken
  scheme: bearer
  sources:
  - openapi/bakkt-crypto-openapi.yml
  type: http
slug: bakkt-authentication
source_filename: bakkt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://bakkt.readme.io/reference/login , https://bakkt.readme.io/docs/getting-started\ndocs: https://bakkt.readme.io/reference/login\nsummary:\n  types:\n  - http-token\n  style: login-endpoint returns bearer security token; token sent in Authorization header on all subsequent\n    HTTPS calls\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: BakktSecurityToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: Clients call POST /apex-crypto/api/v2/login (Crypto Solutions) or Generate Access Token\n    (Fiat/Partner) with a provisioned logonId/password to obtain a short-lived security token, then pass\n    it in the Authorization header on every subsequent request over HTTPS.\n  obtain_operations:\n  - login\n  - generateAccessToken\n  sources:\n  - openapi/bakkt-crypto-openapi.yml\nprovisioning:\n  self_service: false\n  how: Credentials (username, password, environment,\
  \ IP whitelisting) are provisioned per client by contacting\n    sales@bakkt.com; one credential set per client.\n  notes: IP-whitelisted, dedicated per-client API gateway.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/authentication/bakkt-authentication.yml
summary_line: http-token · 1 scheme
tags:
- Company
- Crypto Web3
- Cryptocurrency
- Digital Assets
- Trading
- Payments
- Fiat On-Ramp
- Custody
- Webhooks
- FIX Protocol
---
