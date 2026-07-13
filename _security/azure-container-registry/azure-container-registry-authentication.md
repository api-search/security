---
api_key_in: []
api_specs:
- filename: azure-container-registry-openapi.yaml
  format: yaml
  label: Azure Container Registry
  slug: azure-container-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/openapi/azure-container-registry-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Container Registry Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Container Registry secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Container Registry
provider_slug: azure-container-registry
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-container-registry-openapi.yaml
  type: oauth2
slug: azure-container-registry-authentication
source_filename: azure-container-registry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-container-registry-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow\n  sources:\n  - openapi/azure-container-registry-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/authentication/azure-container-registry-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
---
