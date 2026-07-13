---
api_key_in: []
api_specs:
- filename: azure-dev-ops-openapi.yaml
  format: yaml
  label: Azure DevOps REST API
  slug: azure-devops-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/openapi/azure-dev-ops-openapi.yaml
- filename: azure-dev-ops-openapi.yaml
  format: yaml
  label: Azure DevOps Pipelines API
  slug: azure-devops-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/openapi/azure-dev-ops-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Dev Ops Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure DevOps secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure DevOps
provider_slug: azure-dev-ops
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-dev-ops-openapi.yaml
  type: oauth2
slug: azure-dev-ops-authentication
source_filename: azure-dev-ops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-dev-ops-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow\n  sources:\n  - openapi/azure-dev-ops-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/authentication/azure-dev-ops-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
---
