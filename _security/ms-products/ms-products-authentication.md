---
api_key_in: []
api_specs:
- filename: ms-products-openapi.yml
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ms-products/refs/heads/main/openapi/ms-products-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ms Products Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Products APIs secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Products APIs
provider_slug: ms-products
scheme_count: 1
schemes:
- description: 'Microsoft identity platform OAuth 2.0. Acquire access tokens from https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token and send as `Authorization: Bearer <token>`.'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/ms-products-openapi.yml
  type: oauth2
slug: ms-products-authentication
source_filename: ms-products-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ms-products-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: 'Microsoft identity platform OAuth 2.0. Acquire access tokens from https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    and send as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/ms-products-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ms-products/refs/heads/main/authentication/ms-products-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- Cloud
- Enterprise
- Microsoft
- Office 365
- Productivity
---
