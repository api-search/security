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
name: Microsoft Excel Advanced Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Excel (Advanced) secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Excel (Advanced)
provider_slug: microsoft-excel-advanced
scheme_count: 1
schemes:
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-excel-advanced-openapi.yml
  type: oauth2
slug: microsoft-excel-advanced-authentication
source_filename: microsoft-excel-advanced-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-excel-advanced-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 4\n  description: Microsoft Entra ID OAuth 2.0\n  sources:\n  - openapi/microsoft-excel-advanced-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel-advanced/refs/heads/main/authentication/microsoft-excel-advanced-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Automation
- Business Intelligence
- Data Analysis
- Office
- Spreadsheets
---
