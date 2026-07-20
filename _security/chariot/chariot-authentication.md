---
api_key_in: []
api_specs:
- filename: chariot-openapi-original.yml
  format: yaml
  label: Chariot API
  slug: chariot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chariot/refs/heads/main/openapi/chariot-openapi-original.yml
- filename: chariot-fdx-openapi-original.yml
  format: yaml
  label: Chariot FDX API
  slug: chariot-fdx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chariot/refs/heads/main/openapi/chariot-fdx-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Chariot Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Chariot secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Chariot
provider_slug: chariot
scheme_count: 2
schemes:
- description: OAuth 2.0 Bearer token. A client may hold both scopes, but each FDX authorization must contain exactly one — they are mutually exclusive per authorization. An authorization containing both will be rejected. See the Authentication page for token exchange details.
  flows:
  - authorizationUrl: https://dashboard.givechariot.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.givechariot.com/auth/oauth/token
  name: oauth2
  sources:
  - openapi/chariot-fdx-openapi-original.yml
  type: oauth2
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/chariot-openapi-original.yml
  type: http
slug: chariot-authentication
source_filename: chariot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/chariot-fdx-openapi-original.yml, openapi/chariot-openapi-original.yml, well-known/chariot-openid-configuration.json\ndocs: https://docs.givechariot.com/api/authentication\nnotes: >-\n  Two auth models. The core REST API uses HTTP bearer with secret keys (test prefix sk_test_) over\n  TLS 1.2+ in the Authorization header. The FDX (open-banking) API uses OAuth 2.0 authorization_code.\n  OIDC discovery at /.well-known/openid-configuration advertises grant types authorization_code,\n  refresh_token, client_credentials, and token-exchange; PKCE S256; and private_key_jwt client auth.\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://dashboard.givechariot.com/oauth/authorize\n    tokenUrl: https://api.givechariot.com/auth/oauth/token\n    scopes: 2\n  description: OAuth 2.0 Bearer\
  \ token. A client may hold both scopes, but each FDX authorization\n    must contain exactly one — they are mutually exclusive per authorization. An authorization\n    containing both will be rejected. See the Authentication page for token exchange details.\n  sources:\n  - openapi/chariot-fdx-openapi-original.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/chariot-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chariot/refs/heads/main/authentication/chariot-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Payments
- Donor Advised Funds
- Charitable Giving
- Nonprofit
- Fintech
- DAFpay
- Grants
- Disbursements
- Open Banking
- FDX
- Webhooks
- Company
---
