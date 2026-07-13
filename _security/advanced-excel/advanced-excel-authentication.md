---
api_key_in: []
api_specs:
- filename: microsoft-graph-excel-api-openapi.yml
  format: yaml
  label: Microsoft Graph Excel API
  slug: microsoft-graph-excel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/openapi/microsoft-graph-excel-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Advanced Excel Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Advanced Excel secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Advanced Excel
provider_slug: advanced-excel
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-graph-excel-api-openapi.yml
  type: oauth2
slug: advanced-excel-authentication
source_filename: advanced-excel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-graph-excel-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 2\n  sources:\n  - openapi/microsoft-graph-excel-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/authentication/advanced-excel-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
---
