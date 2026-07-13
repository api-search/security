---
api_key_in: []
api_specs:
- filename: api
  format: yaml
  label: Azure Pipelines REST API
  slug: azure-pipelines-rest-api
  spec_type: OpenAPI
  url: https://dev.azure.com/{organization}/_apis/public/api
- filename: azure-pipelines-build-api-openapi.yml
  format: yaml
  label: Azure Pipelines Build REST API
  slug: azure-pipelines-build-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-pipelines/refs/heads/main/openapi/azure-pipelines-build-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Pipelines Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure Pipelines secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Azure Pipelines
provider_slug: microsoft-azure-pipelines
scheme_count: 2
schemes:
- description: Azure AD OAuth 2.0 bearer token with vso.build scope
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/azure-pipelines-build-api-openapi.yml
  - openapi/azure-pipelines-rest-api-openapi.yml
  type: http
- description: Basic authentication using a Personal Access Token (PAT)
  name: basicAuth
  scheme: basic
  sources:
  - openapi/azure-pipelines-build-api-openapi.yml
  - openapi/azure-pipelines-rest-api-openapi.yml
  type: http
slug: microsoft-azure-pipelines-authentication
source_filename: microsoft-azure-pipelines-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-pipelines-build-api-openapi.yml, openapi/azure-pipelines-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Azure AD OAuth 2.0 bearer token with vso.build scope\n  sources:\n  - openapi/azure-pipelines-build-api-openapi.yml\n  - openapi/azure-pipelines-rest-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication using a Personal Access Token (PAT)\n  sources:\n  - openapi/azure-pipelines-build-api-openapi.yml\n  - openapi/azure-pipelines-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-pipelines/refs/heads/main/authentication/microsoft-azure-pipelines-authentication.yml
summary_line: http · 2 schemes
tags:
- Automation
- Build
- CI/CD
- Deployment
- DevOps
- Pipelines
---
