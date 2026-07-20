---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Blackline Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: BlackLine secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: BlackLine
provider_slug: blackline
scheme_count: 1
schemes:
- credentials:
  - client_id
  - client_secret
  description: BlackLine REST APIs authenticate with OAuth 2.0 client credentials. An application is registered in the BlackLine admin to obtain a Client ID and Client Secret, which are exchanged at the token endpoint for a Bearer access token presented in the Authorization header on each API call.
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  sources:
  - docs
  token_type: Bearer
  token_url: https://api.blackline.com/auth/token
  type: oauth2
slug: blackline-authentication
source_filename: blackline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.blackline.com/apis\ndocs: https://developer.blackline.com/apis\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://api.blackline.com/auth/token\n    grant_type: client_credentials\n    credentials: [client_id, client_secret]\n    token_type: Bearer\n    description: >-\n      BlackLine REST APIs authenticate with OAuth 2.0 client credentials. An\n      application is registered in the BlackLine admin to obtain a Client ID and\n      Client Secret, which are exchanged at the token endpoint for a Bearer\n      access token presented in the Authorization header on each API call.\n    sources: [docs]\nnotes: >-\n  Derived from BlackLine developer portal documentation (no public OpenAPI\n  available to derive securitySchemes from). Token host may be region-specific\n\
  \  in some deployments (SAP Core / STS middleware exchanges an API key for an\n  OAuth Bearer token).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackline/refs/heads/main/authentication/blackline-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- FinOps
- Accounting
- Financial Close
- Reconciliation
- Accounting Automation
- ERP Integration
- Enterprise Software
---
