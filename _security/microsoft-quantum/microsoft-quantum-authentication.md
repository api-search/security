---
api_key_in:
- header
api_specs:
- filename: azure-quantum-data-plane-openapi.json
  format: json
  label: Azure Quantum Workspace Data-Plane API
  slug: azure-quantum-workspace-data-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-quantum/refs/heads/main/openapi/azure-quantum-data-plane-openapi.json
- filename: azure-quantum-resource-manager-openapi.json
  format: json
  label: Azure Quantum Resource Manager API
  slug: azure-quantum-resource-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-quantum/refs/heads/main/openapi/azure-quantum-resource-manager-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Quantum Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- implicit
overview: Microsoft Azure Quantum secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and implicit flow(s).
provider_name: Microsoft Azure Quantum
provider_slug: microsoft-quantum
scheme_count: 3
schemes:
- description: Azure Api-Key Authentication
  in: header
  name: AzureApiKeyAuth
  parameter: x-ms-quantum-api-key
  sources:
  - openapi/azure-quantum-data-plane-openapi.json
  type: apiKey
- description: Azure Entra OAuth2 Authentication
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: AzureEntraAuth
  sources:
  - openapi/azure-quantum-data-plane-openapi.json
  type: oauth2
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-quantum-resource-manager-openapi.json
  type: oauth2
slug: microsoft-quantum-authentication
source_filename: microsoft-quantum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-quantum-data-plane-openapi.json, openapi/azure-quantum-resource-manager-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  - implicit\nschemes:\n- name: AzureApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-ms-quantum-api-key\n  description: Azure Api-Key Authentication\n  sources:\n  - openapi/azure-quantum-data-plane-openapi.json\n- name: AzureEntraAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Azure Entra OAuth2 Authentication\n  sources:\n  - openapi/azure-quantum-data-plane-openapi.json\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n\
  \  - openapi/azure-quantum-resource-manager-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-quantum/refs/heads/main/authentication/microsoft-quantum-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Quantum
- Quantum Computing
- Azure
- Microsoft
- Q#
- QDK
- Resource Estimation
- IonQ
- Quantinuum
- Pasqal
- Rigetti
- Hybrid Quantum
- Fault Tolerance
---
