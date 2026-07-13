---
api_key_in: []
api_specs:
- filename: azure-container-apps-openapi.yml
  format: yaml
  label: Azure Container Apps
  slug: azure-container-apps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/openapi/azure-container-apps-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Container Apps Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Container Apps secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Container Apps
provider_slug: azure-container-apps
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-container-apps-openapi.yml
  type: oauth2
slug: azure-container-apps-authentication
source_filename: azure-container-apps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-container-apps-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  sources:\n  - openapi/azure-container-apps-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/authentication/azure-container-apps-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- Containers
- Dapr
- Kubernetes
- Microservices
- Serverless
---
