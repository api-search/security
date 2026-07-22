---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Silverfin Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Silverfin secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Silverfin
provider_slug: silverfin
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://live.getsilverfin.com/f/{firm_id}/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    tokenUrl: https://live.getsilverfin.com/f/{firm_id}/oauth/token
  name: OAuth2
  sources:
  - https://developer.silverfin.com/reference/authentication
  type: oauth2
slug: silverfin-authentication
source_filename: silverfin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.silverfin.com/reference/authentication\ndocs: https://developer.silverfin.com/reference/authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, refreshToken]\n  token_endpoint: https://live.getsilverfin.com/f/{firm_id}/oauth/token\n  authorization_endpoint: https://live.getsilverfin.com/f/{firm_id}/oauth/authorize\n  access_token_ttl: 2h\n  refresh_token_ttl: 60d\n  notes: >-\n    Silverfin uses OAuth 2.0 (Doorkeeper). Authorization Code grant issues an\n    access token (valid 2 hours) plus a single-use refresh token (valid 60 days\n    as of 2022-08-09). Each refresh token can be used only once; the previous\n    refresh token is revoked as soon as the new access token is first used.\n    Firm-scoped endpoints are namespaced under /f/{firm_id}. A separate SyncAPI\n    authentication path exists for third-party bookkeeping integrations using\n    the financials:transactions:sync scope\
  \ family.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://live.getsilverfin.com/f/{firm_id}/oauth/authorize\n        tokenUrl: https://live.getsilverfin.com/f/{firm_id}/oauth/token\n        grant_types: [authorization_code, refresh_token]\n    sources: [https://developer.silverfin.com/reference/authentication]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silverfin/refs/heads/main/authentication/silverfin-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Business Applications
- Accounting
- Financial Close
- Bookkeeping
- Reporting
- Compliance
- Fintech
- SaaS
- Belgium
---
