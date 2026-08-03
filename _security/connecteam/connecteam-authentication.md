---
api_key_in:
- header
api_specs:
- filename: connecteam-openapi-original.json
  format: json
  label: Connecteam API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connecteam/refs/heads/main/openapi/connecteam-openapi-original.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Connecteam Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Connecteam secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Connecteam
provider_slug: connecteam
scheme_count: 3
schemes:
- description: The Api key of the company given by Connecteam
  in: header
  name: APIKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/connecteam-openapi-original.json
  type: apiKey
- description: OAuth2 Bearer token
  flows:
  - flow: clientCredentials
    scopes: 62
    tokenUrl: /oauth/v1/token
  name: OAuth2
  sources:
  - openapi/connecteam-openapi-original.json
  type: oauth2
- description: Use client_id as Username and client_secret as Password
  name: HTTPBasic
  scheme: basic
  sources:
  - openapi/connecteam-openapi-original.json
  type: http
slug: connecteam-authentication
source_filename: connecteam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://developer.connecteam.com/docs/authentication-1 + openapi/connecteam-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: The Api key of the company given by Connecteam\n  sources:\n  - openapi/connecteam-openapi-original.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/v1/token\n    scopes: 62\n  description: OAuth2 Bearer token\n  sources:\n  - openapi/connecteam-openapi-original.json\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  description: Use client_id as Username and client_secret as Password\n  sources:\n  - openapi/connecteam-openapi-original.json\ndocs:\n- https://developer.connecteam.com/docs/authentication-1\n- https://developer.connecteam.com/docs/oauth-20\n- https://developer.connecteam.com/docs/api-access\n\
  issuance:\n  api_key: Settings -> API Keys -> Add API key (company-wide secret)\n  oauth_app: Your Name -> Integration Center -> OAuth 2.0 -> Create app\ntoken_endpoint: https://api.connecteam.com/oauth/v1/token\ntoken_lifetime_seconds: 86400\nrefresh_token: false\nentitlement: API access requires the Expert plan or higher; the credential only reaches hubs on an eligible\n  plan.\nnotes:\n- The API key is company-wide and unscoped — it is equivalent to a password and grants everything the\n  account's hubs allow. OAuth 2.0 client credentials is the scoped, short-lived alternative and is the\n  correct choice for agents.\n- HTTPBasic is used ONLY to authenticate the token request (client_id as username, client_secret as password);\n  it is not an API-call credential.\n- No OpenID Connect, no /.well-known/oauth-authorization-server metadata, no mTLS.\ncross_ref:\n- scopes/connecteam-scopes.yml\n- conventions/connecteam-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connecteam/refs/heads/main/authentication/connecteam-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Workforce Management
- Human Resources
- Time Tracking
- Scheduling
- Employee Communication
- Task Management
- Forms
- Deskless
- SaaS
---
