---
api_key_in: []
api_specs:
- filename: salesforce-flow-rest-api-openapi.yml
  format: yaml
  label: Salesforce Flow REST API
  slug: salesforce-flow-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-flow/refs/heads/main/openapi/salesforce-flow-rest-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Salesforce Flow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Salesforce Flow secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Salesforce Flow
provider_slug: salesforce-flow
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  sources:
  - openapi/salesforce-flow-rest-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salesforce-flow-rest-api-openapi.yml
  type: http
slug: salesforce-flow-authentication
source_filename: salesforce-flow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-flow-rest-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/salesforce-flow-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/salesforce-flow-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-flow/refs/heads/main/authentication/salesforce-flow-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Automation
- Business Process
- CRM
- Flow
- Process Builder
- Salesforce
- Workflow
---
