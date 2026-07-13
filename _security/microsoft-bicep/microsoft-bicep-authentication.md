---
api_key_in: []
api_specs:
- filename: microsoft-bicep-deployments-openapi.yml
  format: yaml
  label: Bicep Deployments REST API
  slug: bicep-deployments-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bicep/refs/heads/main/openapi/microsoft-bicep-deployments-openapi.yml
- filename: microsoft-bicep-template-specs-openapi.yml
  format: yaml
  label: Bicep Template Specs REST API
  slug: bicep-template-specs-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bicep/refs/heads/main/openapi/microsoft-bicep-template-specs-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Bicep Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Microsoft Bicep secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Microsoft Bicep
provider_slug: microsoft-bicep
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-bicep-deployments-openapi.yml
  - openapi/microsoft-bicep-template-specs-openapi.yml
  type: oauth2
slug: microsoft-bicep-authentication
source_filename: microsoft-bicep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-bicep-deployments-openapi.yml, openapi/microsoft-bicep-template-specs-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow\n  sources:\n  - openapi/microsoft-bicep-deployments-openapi.yml\n  - openapi/microsoft-bicep-template-specs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-bicep/refs/heads/main/authentication/microsoft-bicep-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- ARM Templates
- Azure
- Cloud
- Deployment
- DevOps
- Infrastructure as Code
---
