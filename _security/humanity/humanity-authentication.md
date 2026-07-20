---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Humanity Authentication
name_suffix: Authentication
oauth_flows:
- password
- refresh_token
overview: Humanity secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and refresh_token flow(s).
provider_name: Humanity
provider_slug: humanity
scheme_count: 1
schemes:
- description: 'Humanity v2 API uses OAuth2. An App ID (client_id) and App Secret (client_secret) are created on the Settings > API v2 page. Applications exchange credentials for an access token at the token endpoint. Access tokens expire (expires_in, e.g. 3600 seconds) and are renewed with the refresh_token using grant_type=refresh_token. The token response is JSON: access_token, expires_in, token_type (bearer), scope, refresh_token.'
  flows:
  - flow: password
    grant_type: password
    parameters:
    - client_id
    - client_secret
    - grant_type
    - username
    - password
    - redirect_uri
    tokenUrl: https://www.humanity.com/oauth2/token.php
  - flow: refresh_token
    grant_type: refresh_token
    tokenUrl: https://www.humanity.com/oauth2/token.php
  name: OAuth2
  type: oauth2
slug: humanity-authentication
source_filename: humanity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://platform.humanity.com/docs/getting-started-with-authentication\ndocs: https://platform.humanity.com/docs/getting-started-with-authentication\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\n  - refresh_token\n  token_delivery:\n  - authorization_header_bearer\n  - query_parameter\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Humanity v2 API uses OAuth2. An App ID (client_id) and App Secret\n    (client_secret) are created on the Settings > API v2 page. Applications\n    exchange credentials for an access token at the token endpoint. Access\n    tokens expire (expires_in, e.g. 3600 seconds) and are renewed with the\n    refresh_token using grant_type=refresh_token. The token response is JSON:\n    access_token, expires_in, token_type (bearer), scope, refresh_token.\n  flows:\n  - flow: password\n    tokenUrl: https://www.humanity.com/oauth2/token.php\n    grant_type: password\n    parameters:\n\
  \    - client_id\n    - client_secret\n    - grant_type\n    - username\n    - password\n    - redirect_uri\n  - flow: refresh_token\n    tokenUrl: https://www.humanity.com/oauth2/token.php\n    grant_type: refresh_token\ntoken_usage:\n  header: 'Authorization: Bearer <access_token>'\n  query_parameter: access_token\nnotes: >-\n  Scope is returned as null in the documented token response — the API does not\n  publish a granular OAuth scope surface; authorization is governed by\n  per-endpoint permission levels (3 to 5) tied to the authenticating user's role.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanity/refs/heads/main/authentication/humanity-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Workforce Management
- Employee Scheduling
- Shift Planning
- Time Tracking
- Human Resources
- Leave Management
- Payroll
- Workforce
---
