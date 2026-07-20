---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ermeo Authentication
name_suffix: Authentication
oauth_flows:
- password
- refreshToken
overview: Ermeo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and refreshToken flow(s).
provider_name: Ermeo
provider_slug: ermeo
scheme_count: 1
schemes:
- description: Ermeo secures every API request with an OAuth 2.0 access token passed in the Authorization header as "Bearer {access_token}". Credentials (client_id and client_secret) are issued by the Ermeo team together with a test environment.
  flows:
  - flow: password
    grant_type: password
    parameters:
    - client_id
    - client_secret
    - grant_type=password
    - username
    - password
    token_url: https://api.ermeo.com/oauth/v2/token
  - flow: refreshToken
    grant_type: refresh_token
    parameters:
    - client_id
    - client_secret
    - grant_type=refresh_token
    - refresh_token
    token_url: https://api.ermeo.com/oauth/v2/token
  name: OAuth2
  sources:
  - https://support.en.ermeo.com/login-to-ermeo-api-and-send-requests
  token_url: https://api.ermeo.com/oauth/v2/token
  type: oauth2
slug: ermeo-authentication
source_filename: ermeo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://support.en.ermeo.com/login-to-ermeo-api-and-send-requests\ndocs: https://support.en.ermeo.com/login-to-ermeo-api-and-send-requests\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - password\n  - refreshToken\n  token_type: Bearer\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Ermeo secures every API request with an OAuth 2.0 access token passed in the\n    Authorization header as \"Bearer {access_token}\". Credentials (client_id and\n    client_secret) are issued by the Ermeo team together with a test environment.\n  token_url: https://api.ermeo.com/oauth/v2/token\n  flows:\n  - flow: password\n    grant_type: password\n    token_url: https://api.ermeo.com/oauth/v2/token\n    parameters:\n    - client_id\n    - client_secret\n    - grant_type=password\n    - username\n    - password\n  - flow: refreshToken\n    grant_type: refresh_token\n    token_url: https://api.ermeo.com/oauth/v2/token\n\
  \    parameters:\n    - client_id\n    - client_secret\n    - grant_type=refresh_token\n    - refresh_token\n  sources:\n  - https://support.en.ermeo.com/login-to-ermeo-api-and-send-requests\ntokens:\n  access_token:\n    header: 'Authorization: Bearer {access_token}'\n    lifetime_seconds: 7200\n  refresh_token:\n    lifetime: 2 weeks\n    single_use: true\n    note: A refresh token may be used once to obtain a new access token.\nnotes:\n- Base URL for the API is https://api.ermeo.com\n- No OAuth scope reference is published in the documentation; access is governed by\n  the authenticated user's account permissions rather than granular OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ermeo/refs/heads/main/authentication/ermeo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Field Service Management
- Connected Operator
- Field Operations
- Industrial
- Maintenance
- Inspections
- SaaS
---
