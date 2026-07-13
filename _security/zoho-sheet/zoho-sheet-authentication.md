---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Zoho Sheet Data API
  slug: zoho-sheet-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-sheet/refs/heads/main/openapi/openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zoho Sheet Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
overview: Zoho Sheet secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and implicit flow(s).
provider_name: Zoho Sheet
provider_slug: zoho-sheet
scheme_count: 1
schemes:
- description: Zoho OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
    scopes: 2
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://accounts.zoho.com/oauth/v3/device/token
  name: oauthToken
  sources:
  - openapi/openapi.yml
  type: oauth2
slug: zoho-sheet-authentication
source_filename: zoho-sheet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\nschemes:\n- name: oauthToken\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n    scopes: 2\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    scopes: 2\n  - flow: clientCredentials\n    tokenUrl: https://accounts.zoho.com/oauth/v3/device/token\n    scopes: 2\n  description: Zoho OAuth 2.0 authentication\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-sheet/refs/heads/main/authentication/zoho-sheet-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Spreadsheets
- Productivity
- Collaboration
- Data
- Office
- Zoho
---
