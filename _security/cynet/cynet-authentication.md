---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cynet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cynet secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cynet
provider_slug: cynet
scheme_count: 1
schemes:
- credentials:
  - Access Key (API user)
  - Secret Key (API user, shown only once at creation)
  - Client ID / Site ID
  description: Bearer access token obtained from the account token endpoint. Presented as a header key/value pair on every API call. Valid for 60 minutes, then re-request.
  in: header
  name: cynetAccessToken
  scheme: token
  sources:
  - docs:help.api.cynet.com
  token_endpoint: /api/account/token
  token_method: POST
  token_ttl_seconds: 3600
  type: apiKey
slug: cynet-authentication
source_filename: cynet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://help.api.cynet.com/docs/cynet/b6b6c2d4906e9-authentication\ndocs: https://help.api.cynet.com/docs/cynet/b6b6c2d4906e9-authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  model: token-exchange\n  description: >-\n    Cynet APIs use a short-lived access token. An API user (with the Cynet API User\n    permission, or a role with \"API - full access\") authenticates against the tenant's\n    Cynet API engine to receive a bearer access token that is then presented as a\n    header on every subsequent request. The token is valid for 60 minutes.\nschemes:\n- name: cynetAccessToken\n  type: apiKey\n  in: header\n  scheme: token\n  description: >-\n    Bearer access token obtained from the account token endpoint. Presented as a\n    header key/value pair on every API call. Valid for 60 minutes, then re-request.\n  token_endpoint: /api/account/token\n  token_method: POST\n  token_ttl_seconds:\
  \ 3600\n  credentials:\n    - Access Key (API user)\n    - Secret Key (API user, shown only once at creation)\n    - Client ID / Site ID\n  sources:\n  - docs:help.api.cynet.com\nbase_url_pattern: https://{tenant}.api.cynet.com\nversions:\n- id: v1-on-prem\n  label: On-Prem V1\n  docs: https://help.api.cynet.com/docs/cynet/iah0dsbmetd0e-welcome-to-cynet-api-reference\n- id: v3-saas\n  label: SaaS V3\n  docs: https://help.api.cynet.com/docs/API-V3/9g00cv3m8b10g-cynet-api-documentation\nnotes: >-\n  No OpenID Connect or OAuth 2.0 flow is documented; auth is a custom credential\n  exchange (access key + secret key -> short-lived access token). No public OpenAPI\n  spec is published, so this profile is derived from the Cynet API reference docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cynet/refs/heads/main/authentication/cynet-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cybersecurity
- Security
- XDR
- EDR
- MDR
- SOAR
- Endpoint Security
- Threat Detection
- Incident Response
- MSP
---
