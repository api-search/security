---
api_key_in: []
api_specs:
- filename: compute.json
  format: json
  label: Azure Compute API
  slug: azure-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/compute/resource-manager/Microsoft.Compute/stable/2023-03-01/compute.json
- filename: storage.json
  format: json
  label: Azure Storage API
  slug: azure-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/storage/resource-manager/Microsoft.Storage/stable/2023-01-01/storage.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Cloud Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Azure Cloud secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Azure Cloud
provider_slug: azure-cloud
scheme_count: 1
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token (scope https://management.azure.com/.default)
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  sources:
  - openapi/azure-cloud-openapi.yml
  type: oauth2
slug: azure-cloud-authentication
source_filename: azure-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-cloud-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: entra\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0 bearer token (scope https://management.azure.com/.default)\n  sources:\n  - openapi/azure-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-cloud/refs/heads/main/authentication/azure-cloud-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- AI
- Cloud Computing
- Databases
- IaaS
- Infrastructure
- Machine Learning
- Microsoft
- Networking
- PaaS
- Platform as a Service
- SaaS
- Storage
---
