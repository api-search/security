---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ms Office Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Office APIs secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Office APIs
provider_slug: ms-office
scheme_count: 1
schemes:
- description: Microsoft identity platform OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/ms-office-openapi.yml
  type: oauth2
slug: ms-office-authentication
source_filename: ms-office-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ms-office-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 5\n  description: Microsoft identity platform OAuth 2.0\n  sources:\n  - openapi/ms-office-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ms-office/refs/heads/main/authentication/ms-office-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Collaboration
- Documents
- Microsoft
- Office
- Productivity
---
