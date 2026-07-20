---
api_key_in: []
api_specs:
- filename: microsoft-excel-graph-api.yaml
  format: yaml
  label: Microsoft Graph Excel API
  slug: microsoft-graph-excel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/openapi/microsoft-excel-graph-api.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Microsoft Excel Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Excel secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Excel
provider_slug: microsoft-excel
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization using Microsoft Identity Platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-excel-graph-api.yaml
  type: oauth2
slug: microsoft-excel-authentication
source_filename: microsoft-excel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/microsoft-excel-graph-api.yaml\ndocs: https://learn.microsoft.com/en-us/graph/auth/\nnote: >-\n  OAuth 2.0 via the Microsoft identity platform (Microsoft Entra ID). Delegated\n  (authorization code / PKCE) and app-only (client credentials) flows are supported; Excel\n  workbook access requires Files.* / Sites.* scopes (see scopes/). Tokens are acquired from\n  login.microsoftonline.com and presented as Bearer tokens on graph.microsoft.com.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 2\n  description: OAuth 2.0 authorization using Microsoft Identity Platform\n  sources:\n  - openapi/microsoft-excel-graph-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/authentication/microsoft-excel-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Automation
- Data Analysis
- Microsoft
- Microsoft 365
- Office
- Spreadsheets
---
