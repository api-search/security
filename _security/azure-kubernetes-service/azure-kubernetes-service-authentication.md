---
api_key_in: []
api_specs:
- filename: azure-kubernetes-service-openapi.yml
  format: yaml
  label: Azure Kubernetes Service REST API
  slug: azure-kubernetes-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/openapi/azure-kubernetes-service-openapi.yml
- filename: azure-kubernetes-service-openapi.yml
  format: yaml
  label: Azure Kubernetes Service Managed Clusters API
  slug: azure-kubernetes-service-managed-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/openapi/azure-kubernetes-service-openapi.yml
- filename: azure-kubernetes-service-openapi.yml
  format: yaml
  label: Azure Kubernetes Service Agent Pools API
  slug: azure-kubernetes-service-agent-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/openapi/azure-kubernetes-service-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Kubernetes Service Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Kubernetes Service secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-kubernetes-service-openapi.yml
  type: oauth2
slug: azure-kubernetes-service-authentication
source_filename: azure-kubernetes-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-kubernetes-service-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/azure-kubernetes-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/authentication/azure-kubernetes-service-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
---
