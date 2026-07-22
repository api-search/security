---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Makeleaps Authentication
name_suffix: Authentication
oauth_flows: []
overview: MakeLeaps declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MakeLeaps
provider_slug: makeleaps
scheme_count: 1
schemes:
- description: 'OAuth 2.0 client-credentials grant. The client posts base64(client_id:client_secret) in a Basic Authorization header to the token endpoint to obtain a short-lived Bearer access token, then sends that token as `Authorization: Bearer {access_token}` on every subsequent API request.'
  flow: clientCredentials
  id: oauth2_client_credentials
  notes: 'Requests are partner-scoped: the authenticated partner''s MID is inserted into the path as /api/partner/{partner_mid}/... No explicit OAuth scope parameter is documented in the public tutorials.'
  request_header: 'Authorization: Bearer {access_token}'
  scopes: []
  token_request:
    body: grant_type=client_credentials
    content_type: application/x-www-form-urlencoded
    header: 'Authorization: Basic base64(client_id:client_secret)'
    method: POST
  token_url: https://api.makeleaps.com/user/oauth2/token/
  type: oauth2
slug: makeleaps-authentication
source_filename: makeleaps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.makeleaps.com/en/api/tutorial/sending-your-first-document-with-makeleaps/\napi: MakeLeaps API\nbase_url: https://api.makeleaps.com\nschemes:\n- id: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    OAuth 2.0 client-credentials grant. The client posts base64(client_id:client_secret)\n    in a Basic Authorization header to the token endpoint to obtain a short-lived\n    Bearer access token, then sends that token as `Authorization: Bearer {access_token}`\n    on every subsequent API request.\n  token_url: https://api.makeleaps.com/user/oauth2/token/\n  token_request:\n    method: POST\n    header: 'Authorization: Basic base64(client_id:client_secret)'\n    content_type: application/x-www-form-urlencoded\n    body: grant_type=client_credentials\n  request_header: 'Authorization: Bearer {access_token}'\n  scopes: []\n  notes: >-\n    Requests are partner-scoped: the authenticated\
  \ partner's MID is inserted into the\n    path as /api/partner/{partner_mid}/... No explicit OAuth scope parameter is\n    documented in the public tutorials.\ncredentials_required:\n- client_id\n- client_secret\n- partner_mid\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makeleaps/refs/heads/main/authentication/makeleaps-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Invoicing
- Billing
- Accounting
- Finance
- Payments
- Document Management
- E-Invoicing
- SaaS
- Japan
- Ricoh
---
