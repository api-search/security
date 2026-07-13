---
api_key_in: []
api_specs:
- filename: salesforce-automation-flow-openapi.yml
  format: yaml
  label: Salesforce Flow Automation API
  slug: salesforce-flow-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation-system/refs/heads/main/openapi/salesforce-automation-flow-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Salesforce Automation System Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Salesforce Automation System secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Salesforce Automation System
provider_slug: salesforce-automation-system
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  sources:
  - openapi/salesforce-automation-flow-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salesforce-automation-flow-openapi.yml
  type: http
slug: salesforce-automation-system-authentication
source_filename: salesforce-automation-system-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-automation-flow-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    scopes: 2\n  - flow: clientCredentials\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/salesforce-automation-flow-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/salesforce-automation-flow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation-system/refs/heads/main/authentication/salesforce-automation-system-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Approval Process
- Automation
- CRM
- Flow
- Process Builder
- Salesforce
- Workflow
---
