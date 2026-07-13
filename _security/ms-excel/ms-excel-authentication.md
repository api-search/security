---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Excel API
  slug: microsoft-graph-excel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ms Excel Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Excel API secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Excel API
provider_slug: ms-excel
scheme_count: 1
schemes:
- description: Microsoft identity platform OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/ms-excel-openapi.yml
  type: oauth2
slug: ms-excel-authentication
source_filename: ms-excel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ms-excel-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 2\n  description: Microsoft identity platform OAuth 2.0\n  sources:\n  - openapi/ms-excel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ms-excel/refs/heads/main/authentication/ms-excel-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Data Analysis
- Excel
- Microsoft Graph
- Office 365
- Spreadsheets
---
