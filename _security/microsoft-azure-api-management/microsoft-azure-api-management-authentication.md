---
api_key_in: []
api_specs:
- filename: microsoft-azure-api-management-rest-api-openapi.yaml
  format: yaml
  label: Azure API Management REST API
  slug: azure-api-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/openapi/microsoft-azure-api-management-rest-api-openapi.yaml
- filename: microsoft-azure-api-management-gateway-openapi.yaml
  format: yaml
  label: Azure API Management Gateway
  slug: azure-api-management-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/openapi/microsoft-azure-api-management-gateway-openapi.yaml
- filename: microsoft-azure-api-management-self-hosted-gateway-openapi.yaml
  format: yaml
  label: Azure API Management Self-Hosted Gateway
  slug: azure-api-management-self-hosted-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/openapi/microsoft-azure-api-management-self-hosted-gateway-openapi.yaml
- filename: microsoft-azure-api-management-ai-gateway-openapi.yaml
  format: yaml
  label: Azure API Management AI Gateway
  slug: azure-api-management-ai-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/openapi/microsoft-azure-api-management-ai-gateway-openapi.yaml
- filename: microsoft-azure-api-management-developer-portal-openapi.yaml
  format: yaml
  label: Azure API Management Developer Portal
  slug: azure-api-management-developer-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/openapi/microsoft-azure-api-management-developer-portal-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Api Management Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Microsoft Azure API Management secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Microsoft Azure API Management
provider_slug: microsoft-azure-api-management
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-api-management-rest-api-openapi.yaml
  type: oauth2
slug: microsoft-azure-api-management-authentication
source_filename: microsoft-azure-api-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-api-management-rest-api-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  sources:\n  - openapi/microsoft-azure-api-management-rest-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/authentication/microsoft-azure-api-management-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- A2A
- AI Gateway
- API Center
- API Gateway
- API Management
- Enterprise
- MCP
- Microsoft Azure
---
