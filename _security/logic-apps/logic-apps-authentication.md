---
api_key_in: []
api_specs:
- filename: logic-apps-management-api-openapi.yml
  format: yaml
  label: Azure Logic Apps Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logic-apps/refs/heads/main/openapi/logic-apps-management-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Logic Apps Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Azure Logic Apps secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Azure Logic Apps
provider_slug: logic-apps
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/token
  name: azureAD
  sources:
  - openapi/logic-apps-management-api-openapi.yml
  type: oauth2
slug: logic-apps-authentication
source_filename: logic-apps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/logic-apps-management-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: azureAD\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/logic-apps-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logic-apps/refs/heads/main/authentication/logic-apps-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- Enterprise
- iPaaS
- Integration
- Microsoft
- Workflow Automation
---
