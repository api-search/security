---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ikas Ikas Teknoloji As Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Ikas, IKAS Teknoloji AS secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Ikas, IKAS Teknoloji AS
provider_slug: ikas-ikas-teknoloji-as
scheme_count: 1
schemes:
- description: ikas apps authenticate with OAuth 2.0. Private (store-specific) apps use the client_credentials flow; public admin apps use the authorization_code flow. Access tokens are sent as an HTTP Bearer token on GraphQL requests and expire after 14400 seconds (4 hours).
  flows:
  - flow: clientCredentials
    request:
      content_type: application/x-www-form-urlencoded
      params:
      - grant_type=client_credentials
      - client_id
      - client_secret
    response_fields:
    - access_token
    - token_type
    - expires_in
    tokenUrl: https://{store_name}.myikas.com/api/admin/oauth/token
    used_by: private apps
  - docs: https://builders.ikas.com/docs/app-development
    flow: authorizationCode
    used_by: public admin apps
  name: OAuth2
  scopes_ref: scopes/ikas-ikas-teknoloji-as-scopes.yml
  type: oauth2
slug: ikas-ikas-teknoloji-as-authentication
source_filename: ikas-ikas-teknoloji-as-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://ikas.dev/docs/api/getting-started/authentication\ndocs: https://ikas.dev/docs/api/getting-started/authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  token_style: bearer\n  token_ttl_seconds: 14400\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    ikas apps authenticate with OAuth 2.0. Private (store-specific) apps use the\n    client_credentials flow; public admin apps use the authorization_code flow.\n    Access tokens are sent as an HTTP Bearer token on GraphQL requests and\n    expire after 14400 seconds (4 hours).\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{store_name}.myikas.com/api/admin/oauth/token\n    used_by: private apps\n    request:\n      content_type: application/x-www-form-urlencoded\n      params: [grant_type=client_credentials, client_id, client_secret]\n    response_fields: [access_token, token_type, expires_in]\n\
  \  - flow: authorizationCode\n    used_by: public admin apps\n    docs: https://builders.ikas.com/docs/app-development\n  scopes_ref: scopes/ikas-ikas-teknoloji-as-scopes.yml\napi_request:\n  endpoint: https://api.myikas.com/api/v1/admin/graphql\n  header: 'Authorization: Bearer <access_token>'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ikas-ikas-teknoloji-as/refs/heads/main/authentication/ikas-ikas-teknoloji-as-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- E-commerce
- Retail
- Storefront
- Orders
- Products
- Inventory
- GraphQL
- Webhooks
- OAuth
- SDK
- MCP
---
