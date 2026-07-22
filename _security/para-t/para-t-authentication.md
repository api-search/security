---
api_key_in: []
api_specs:
- filename: para-t-openapi-original.yml
  format: yaml
  label: Paraşüt API V4
  slug: paraşüt-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/para-t/refs/heads/main/openapi/para-t-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Para T Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: Paraşüt secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: Paraşüt
provider_slug: para-t
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.parasut.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.parasut.com/oauth/token
  - flow: password
    notes: grant_type=password with client_id, client_secret, username, password, redirect_uri=urn:ietf:wg:oauth:2.0:oob
    tokenUrl: https://api.parasut.com/oauth/token
  name: parasut_auth
  sources:
  - openapi/para-t-openapi-original.yml
  type: oauth2
slug: para-t-authentication
source_filename: para-t-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/para-t-openapi-original.yml\ndocs: https://apidocs.parasut.com/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - password\n  token_lifetime: 2h\n  refresh: rotating refresh_token\n  header: 'Authorization: Bearer <access_token>'\n  credential_provisioning: client_id/client_secret requested from destek@parasut.com\nschemes:\n- name: parasut_auth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.parasut.com/oauth/authorize\n    tokenUrl: https://api.parasut.com/oauth/token\n    scopes: 0\n  - flow: password\n    tokenUrl: https://api.parasut.com/oauth/token\n    notes: 'grant_type=password with client_id, client_secret, username, password, redirect_uri=urn:ietf:wg:oauth:2.0:oob'\n  sources:\n  - openapi/para-t-openapi-original.yml\nnotes: >\n  Bearer access_token is valid for 2 hours; refresh with the rotating refresh_token\n  (a new refresh_token is\
  \ returned on each refresh). No OAuth scopes are defined — a\n  successful token grants full access within the company (firma_no) scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/para-t/refs/heads/main/authentication/para-t-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Accounting
- Pre-Accounting
- e-Invoicing
- Invoicing
- Fintech
- SaaS
- Turkey
- ERP
- JSON:API
---
