---
api_key_in: []
api_specs:
- filename: azure-logic-apps-openapi.yaml
  format: yaml
  label: Azure Logic Apps
  slug: azure-logic-apps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/openapi/azure-logic-apps-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Logic Apps Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Logic Apps secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-logic-apps-openapi.yaml
  type: oauth2
slug: azure-logic-apps-authentication
source_filename: azure-logic-apps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-logic-apps-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/azure-logic-apps-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/authentication/azure-logic-apps-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- Integration
- iPaaS
- Workflows
---
