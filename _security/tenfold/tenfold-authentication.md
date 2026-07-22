---
api_key_in: []
api_specs:
- filename: tenfold-openapi.yml
  format: yaml
  label: Tenfold API
  slug: tenfold-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenfold/refs/heads/main/openapi/tenfold-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tenfold Authentication
name_suffix: Authentication
oauth_flows:
- password
- clientCredentials
overview: Tenfold secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and clientCredentials flow(s).
provider_name: Tenfold
provider_slug: tenfold
scheme_count: 3
schemes:
- flow: password
  name: oauth2Password
  sources:
  - openapi/tenfold-openapi.yml
  tokenUrl: https://api.tenfold.com/v2/oauth/token
  type: oauth2
- flow: clientCredentials
  name: oauth2ClientCredentials
  sources:
  - openapi/tenfold-openapi.yml
  tokenUrl: https://api.tenfold.com/v2/oauth/token
  type: oauth2
- bearerFormat: JWT
  login_endpoint: https://api.tenfold.com/v2/users/login
  name: bearerJWT
  scheme: bearer
  sources:
  - openapi/tenfold-openapi.yml
  type: http
slug: tenfold-authentication
source_filename: tenfold-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://apidocs.tenfold.com/\ndocs: https://apidocs.tenfold.com/\nsummary:\n  types: [oauth2, http]\n  http_schemes: [bearer]\n  oauth2_flows: [password, clientCredentials]\n  notes: >-\n    Tenfold supports OAuth 2.0 (Resource Owner Password Credentials and Client\n    Credentials grants) across v1 and v2, and a JWT bearer token obtained from\n    /v2/users/login. v2 primarily uses JWT presented as\n    \"Authorization: Bearer JWT <token>\". OAuth access tokens are presented as\n    \"Authorization: Bearer <token>\". No OAuth scope catalog is documented.\nschemes:\n  - name: oauth2Password\n    type: oauth2\n    flow: password\n    tokenUrl: https://api.tenfold.com/v2/oauth/token\n    sources: [openapi/tenfold-openapi.yml]\n  - name: oauth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://api.tenfold.com/v2/oauth/token\n    sources: [openapi/tenfold-openapi.yml]\n  - name: bearerJWT\n\
  \    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    login_endpoint: https://api.tenfold.com/v2/users/login\n    sources: [openapi/tenfold-openapi.yml]\ntoken_endpoints:\n  v1: POST https://api.tenfold.com/api/v1/oauth/token\n  v2: PUT https://api.tenfold.com/v2/oauth/token\n  jwt_login: POST https://api.tenfold.com/v2/users/login\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenfold/refs/heads/main/authentication/tenfold-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Company
- CTI
- Contact Center
- Telephony
- CRM Integration
- Call Analytics
- Customer Experience
- Voice
---
