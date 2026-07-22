---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Poynt Authentication
name_suffix: Authentication
oauth_flows:
- jwt-bearer
overview: Poynt secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the jwt-bearer flow(s).
provider_name: Poynt
provider_slug: poynt
scheme_count: 1
schemes:
- description: 'Apps authenticate with a self-signed JWT (signed with the application''s RSA private key registered with Poynt) which is POSTed to the token endpoint and exchanged for a short-lived OAuth 2.0 access token. The access token is then sent as an Authorization: Bearer <access-token> header on every API request, alongside an Api-Version header.'
  grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer
  name: OAuth2 self-signed JWT bearer
  request_headers:
  - 'Authorization: Bearer <access-token>'
  - 'Api-Version: 1.2'
  - 'Content-Type: application/json'
  scheme: bearer
  sources:
  - docs.poynt.com/api-reference
  token_url: https://services.poynt.net/token
  type: oauth2
slug: poynt-authentication
source_filename: poynt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.poynt.com/app-integration/\ndocs: https://docs.poynt.com/api-reference/index.html\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - jwt-bearer\n  api_key_in: []\nschemes:\n- name: OAuth2 self-signed JWT bearer\n  type: oauth2\n  scheme: bearer\n  description: 'Apps authenticate with a self-signed JWT (signed with the application''s\n    RSA private key registered with Poynt) which is POSTed to the token endpoint and\n    exchanged for a short-lived OAuth 2.0 access token. The access token is then sent\n    as an Authorization: Bearer <access-token> header on every API request, alongside\n    an Api-Version header.'\n  token_url: https://services.poynt.net/token\n  grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\n  request_headers:\n  - 'Authorization: Bearer <access-token>'\n  - 'Api-Version: 1.2'\n  - 'Content-Type: application/json'\n  sources:\n  - docs.poynt.com/api-reference\nnotes: 'Poynt uses\
  \ application-level authorization (an app is granted access to a\n  merchant business at onboarding) rather than fine-grained OAuth scopes, so there\n  is no published OAuth scope reference.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poynt/refs/heads/main/authentication/poynt-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Consumer
- Payments
- Point of Sale
- Commerce
- Merchant Services
- Payment Processing
- Developer Platform
---
