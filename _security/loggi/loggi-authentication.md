---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Loggi Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Loggi secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Loggi
provider_slug: loggi
scheme_count: 2
schemes:
- applied_as: Authorization header on all API requests
  flow: clientCredentials
  name: OAuth2ClientCredentials
  request_fields:
  - client_id
  - client_secret
  returns: JWT bearer token
  source: https://docs.api.loggi.com/reference/authenticatev2
  token_urls:
    production: https://api.loggi.com/v2/oauth2/token
    staging: https://stg.api.loggi.com/v2/oauth2/token
  type: oauth2
- deprecated: true
  field: idToken
  in: header
  name: AuthV1Deprecated
  parameter: Authorization
  source: https://docs.api.loggi.com/reference/authenticatev1
  type: apiKey
slug: loggi-authentication
source_filename: loggi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.api.loggi.com/reference/authenticatev2\ndocs: https://docs.api.loggi.com/reference/authenticatev2\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_format: JWT\n  token_header: Authorization\nnotes: >-\n  Loggi uses OAuth2 client-credentials style authentication. The integrator\n  exchanges a client_id + client_secret at the AuthAPI token endpoint and\n  receives a JWT that is sent in the Authorization header on every subsequent\n  request to Loggi's APIs. Authentication V1 (idToken in the Authorization\n  header) is deprecated in favor of V2. Developers must never request a third\n  party's client_id/client_secret; sellers provide only an integration_code.\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_urls:\n      production: https://api.loggi.com/v2/oauth2/token\n      staging: https://stg.api.loggi.com/v2/oauth2/token\n    request_fields:\
  \ [client_id, client_secret]\n    returns: JWT bearer token\n    applied_as: Authorization header on all API requests\n    source: https://docs.api.loggi.com/reference/authenticatev2\n  - name: AuthV1Deprecated\n    type: apiKey\n    in: header\n    parameter: Authorization\n    field: idToken\n    deprecated: true\n    source: https://docs.api.loggi.com/reference/authenticatev1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/authentication/loggi-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Logistics
- Shipping
- Last-Mile Delivery
- Freight
- Tracking
- Brazil
---
