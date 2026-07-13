---
api_key_in: []
api_specs:
- filename: azure-management-openapi.yaml
  format: yaml
  label: Azure Compute API
  slug: azure-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/openapi/azure-management-openapi.yaml
- filename: azure-management-openapi.yaml
  format: yaml
  label: Azure Storage API
  slug: azure-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/openapi/azure-management-openapi.yaml
- filename: azure-management-openapi.yaml
  format: yaml
  label: Azure Cognitive Services API
  slug: azure-cognitive-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/openapi/azure-management-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Microsoft Azure secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Microsoft Azure
provider_slug: azure
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-management-openapi.yaml
  type: oauth2
slug: azure-authentication
source_filename: azure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-management-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  sources:\n  - openapi/azure-management-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/authentication/azure-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud Computing
- Databases
- Infrastructure
- Machine Learning
- Networking
- Platform as a Service
- Storage
---
