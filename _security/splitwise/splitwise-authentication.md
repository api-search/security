---
api_key_in: []
api_specs:
- filename: splitwise-openapi.json
  format: json
  label: Splitwise API
  slug: splitwise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Splitwise Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Splitwise secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Splitwise
provider_slug: splitwise
scheme_count: 2
schemes:
- description: 'Splitwise uses OAuth 2 with the authorization code flow. To connect via OAuth 2, you''ll need to [register your app](https://secure.splitwise.com/apps). When you register, you''ll be given a key and secret.


    **Note**: OAuth can be a very confusing protocol to implement correctly, and we **strongly** recommend

    that you use an existing OAuth library to connect to Splitwise. You can find a list of OAut'
  flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: /oauth/token
  name: OAuth
  sources:
  - openapi/splitwise-openapi.json
  type: oauth2
- bearerFormat: API key
  description: 'For speed and ease of prototyping, you can generate a personal API key on your app''s details page. You should present this key to the server via the Authorization header as a Bearer token. The API key is an access token for your personal account, so keep it as safe as you would a password.

    If your key becomes compromised or you want to invalidate your existing key for any other reason, you can do '
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/splitwise-openapi.json
  type: http
slug: splitwise-authentication
source_filename: splitwise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/splitwise-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n    scopes: 0\n  description: |-\n    Splitwise uses OAuth 2 with the authorization code flow. To connect via OAuth 2, you'll need to [register your app](https://secure.splitwise.com/apps). When you register, you'll be given a key and secret.\n\n    **Note**: OAuth can be a very confusing protocol to implement correctly, and we **strongly** recommend\n    that you use an existing OAuth library to connect to Splitwise. You can find a list of OAut\n  sources:\n  - openapi/splitwise-openapi.json\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: \"For speed and ease of prototyping, you can generate a personal API key on your\\\n\
  \    \\ app's details page. You should present this key to the server via the Authorization header\\\n    \\ as a Bearer token. The API key is an access token for your personal account, so keep it\\\n    \\ as safe as you would a password.\\nIf your key becomes compromised or you want to invalidate\\\n    \\ your existing key for any other reason, you can do \"\n  sources:\n  - openapi/splitwise-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/authentication/splitwise-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Consumer
- Expense Management
- Personal Finance
- Bill Splitting
- Payments
- REST API
- OAuth
---
