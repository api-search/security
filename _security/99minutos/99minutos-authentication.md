---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: 99Minutos Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: 99minutos secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: 99minutos
provider_slug: 99minutos
scheme_count: 1
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  notes: 99minutos issues API credentials (client_id / client_secret) per merchant account. POST them to /api/v3/oauth/token to obtain a bearer access_token that expires after ~60 minutes.
  request_body:
  - client_id
  - client_secret
  response_fields:
  - access_token
  - token_type
  sandbox_token_url: https://sandbox.99minutos.com/api/v3/oauth/token
  token_url: https://api.99minutos.com/api/v3/oauth/token
  type: oauth2
  usage: 'Send the returned access_token as an "Authorization: Bearer <access_token>" header on all /api/v3 requests.'
slug: 99minutos-authentication
source_filename: 99minutos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developers.99minutos.com/reference/oauth_token_create\ndocs: https://developers.99minutos.com/recipes/autenticarse-login\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_type: bearer\n  token_lifetime: 3600  # access_token valid ~60 minutes\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://api.99minutos.com/api/v3/oauth/token\n    sandbox_token_url: https://sandbox.99minutos.com/api/v3/oauth/token\n    request_body: [client_id, client_secret]\n    response_fields: [access_token, token_type]\n    usage: 'Send the returned access_token as an \"Authorization: Bearer <access_token>\" header on all /api/v3 requests.'\n    notes: >-\n      99minutos issues API credentials (client_id / client_secret) per merchant account.\n      POST them to /api/v3/oauth/token to obtain a bearer access_token that expires after ~60 minutes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/99minutos/refs/heads/main/authentication/99minutos-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Logistics
- Shipping
- Last-Mile Delivery
- Ecommerce
- Fulfillment
- Package Tracking
- Latin America
- Parcel Delivery
- Webhooks
---
