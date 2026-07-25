---
api_key_in: []
api_specs:
- filename: microsoft-azure-pipelines-artifacts-api-openapi.yml
  format: yaml
  label: Azure Pipelines Artifacts API
  slug: microsoft-azure-pipelines-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-pipelines/refs/heads/main/openapi/microsoft-azure-pipelines-artifacts-api-openapi.yml
- filename: microsoft-azure-pipelines-build-artifacts-api-openapi.yml
  format: yaml
  label: Azure Pipelines Build Artifacts API
  slug: microsoft-azure-pipelines-build-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-pipelines/refs/heads/main/openapi/microsoft-azure-pipelines-build-artifacts-api-openapi.yml
- filename: microsoft-azure-pipelines-build-definitions-api-openapi.yml
  format: yaml
  label: Azure Pipelines Build Definitions API
  slug: microsoft-azure-pipelines-build-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-pipelines/refs/heads/main/openapi/microsoft-azure-pipelines-build-definitions-api-openapi.yml
- filename: microsoft-azure-pipelines-build-tags-api-openapi.yml
  format: yaml
  label: Azure Pipelines Build Tags API
  slug: microsoft-azure-pipelines-build-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-pipelines/refs/heads/main/openapi/microsoft-azure-pipelines-build-tags-api-openapi.yml
- filename: microsoft-azure-pipelines-builds-api-openapi.yml
  format: yaml
  label: Azure Pipelines Builds API
  slug: microsoft-azure-pipelines-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-pipelines/refs/heads/main/openapi/microsoft-azure-pipelines-builds-api-openapi.yml
- filename: microsoft-azure-pipelines-logs-api-openapi.yml
  format: yaml
  label: Azure Pipelines Logs API
  slug: microsoft-azure-pipelines-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-pipelines/refs/heads/main/openapi/microsoft-azure-pipelines-logs-api-openapi.yml
- filename: microsoft-azure-pipelines-pipelines-api-openapi.yml
  format: yaml
  label: Azure Pipelines Pipelines API
  slug: microsoft-azure-pipelines-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-pipelines/refs/heads/main/openapi/microsoft-azure-pipelines-pipelines-api-openapi.yml
- filename: microsoft-azure-pipelines-runs-api-openapi.yml
  format: yaml
  label: Azure Pipelines Runs API
  slug: microsoft-azure-pipelines-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-pipelines/refs/heads/main/openapi/microsoft-azure-pipelines-runs-api-openapi.yml
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
