---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Everlance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Everlance secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Everlance
provider_slug: everlance
scheme_count: 1
schemes:
- description: 'Everlance Business API requires an access_token passed in the Authorization header as: "Authorization: Bearer access_token". The token is provisioned by the Everlance team (not self-service). Static long-lived bearer token — no OAuth2 flow or scope surface is documented.'
  format: Bearer {access_token}
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - docs
  type: http
slug: everlance-authentication
source_filename: everlance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://help.everlance.com/hc/en-us/articles/45326074722203-Managing-Data-with-APIs\ndocs: https://help.everlance.com/hc/en-us/sections/38201888806157-Everlance-Business-API\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  access_model: gated\n  provisioning: 'Access tokens are issued by the Everlance team on request. Ask your\n    Everlance account manager or email support@everlance.com to obtain an API access\n    token.'\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Everlance Business API requires an access_token passed in the Authorization\n    header as: \"Authorization: Bearer access_token\". The token is provisioned by the\n    Everlance team (not self-service). Static long-lived bearer token — no OAuth2 flow\n    or scope surface is documented.'\n  in: header\n  header: Authorization\n  format: 'Bearer {access_token}'\n  sources:\n \
  \ - docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everlance/refs/heads/main/authentication/everlance-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Mileage Tracking
- Expense Management
- Reimbursement
- Fleet Management
- Tax
- Gig Economy
- HR Integration
- Business API
---
