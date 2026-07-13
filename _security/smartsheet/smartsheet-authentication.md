---
api_key_in: []
api_specs:
- filename: smartsheet-openapi.yml
  format: yaml
  label: Smartsheet REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartsheet/refs/heads/main/openapi/smartsheet-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Smartsheet Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Smartsheet secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Smartsheet
provider_slug: smartsheet
scheme_count: 2
schemes:
- description: Smartsheet API access token sent in the Authorization header as a Bearer token.
  name: ApiToken
  scheme: bearer
  sources:
  - openapi/smartsheet-openapi.yml
  type: http
- description: Smartsheet OAuth 2.0 authorization.
  flows:
  - authorizationUrl: https://app.smartsheet.com/b/authorize
    flow: authorizationCode
    scopes: 10
    tokenUrl: https://api.smartsheet.com/2.0/token
  name: OAuth2
  sources:
  - openapi/smartsheet-openapi.yml
  type: oauth2
slug: smartsheet-authentication
source_filename: smartsheet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smartsheet-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiToken\n  type: http\n  scheme: bearer\n  description: Smartsheet API access token sent in the Authorization header as a Bearer token.\n  sources:\n  - openapi/smartsheet-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.smartsheet.com/b/authorize\n    tokenUrl: https://api.smartsheet.com/2.0/token\n    scopes: 10\n  description: Smartsheet OAuth 2.0 authorization.\n  sources:\n  - openapi/smartsheet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartsheet/refs/heads/main/authentication/smartsheet-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Work Management
- Project Management
- Collaboration
- Productivity
- Workflow Automation
- Spreadsheets
---
