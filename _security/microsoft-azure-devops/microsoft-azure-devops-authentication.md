---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Azure DevOps Services REST API
  slug: azure-devops-services-rest-api
  spec_type: OpenAPI
  url: https://learn.microsoft.com/en-us/rest/api/azure/devops/
- filename: azure-devops-work-items-api-openapi.yml
  format: yaml
  label: Azure DevOps Boards API
  slug: azure-devops-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-work-items-api-openapi.yml
- filename: azure-devops-git-api-openapi.yml
  format: yaml
  label: Azure DevOps Repos API
  slug: azure-devops-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-git-api-openapi.yml
- filename: azure-devops-pipelines-api-openapi.yml
  format: yaml
  label: Azure DevOps Pipelines API
  slug: azure-devops-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-pipelines-api-openapi.yml
- filename: azure-devops-builds-api-openapi.yml
  format: yaml
  label: Azure DevOps Build API
  slug: azure-devops-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-builds-api-openapi.yml
- filename: azure-devops-releases-api-openapi.yml
  format: yaml
  label: Azure DevOps Release API
  slug: azure-devops-release-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-releases-api-openapi.yml
- filename: azure-devops-test-plans-api-openapi.yml
  format: yaml
  label: Azure DevOps Test Plans API
  slug: azure-devops-test-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-test-plans-api-openapi.yml
- filename: azure-devops-artifacts-api-openapi.yml
  format: yaml
  label: Azure DevOps Artifacts API
  slug: azure-devops-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-artifacts-api-openapi.yml
- filename: azure-devops-service-hooks-api-openapi.yml
  format: yaml
  label: Azure DevOps Service Hooks API
  slug: azure-devops-service-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-service-hooks-api-openapi.yml
- filename: azure-devops-wiki-api-openapi.yml
  format: yaml
  label: Azure DevOps Wiki API
  slug: azure-devops-wiki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/openapi/azure-devops-wiki-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Devops Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure DevOps secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Azure DevOps
provider_slug: microsoft-azure-devops
scheme_count: 2
schemes:
- description: Azure AD OAuth 2.0 bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/azure-devops-artifacts-api-openapi.yml
  - openapi/azure-devops-builds-api-openapi.yml
  - openapi/azure-devops-git-api-openapi.yml
  - openapi/azure-devops-pipelines-api-openapi.yml
  - openapi/azure-devops-releases-api-openapi.yml
  - openapi/azure-devops-service-hooks-api-openapi.yml
  - openapi/azure-devops-test-plans-api-openapi.yml
  - openapi/azure-devops-wiki-api-openapi.yml
  - openapi/azure-devops-work-items-api-openapi.yml
  type: http
- description: Basic authentication using a Personal Access Token (PAT). Use any string as the username and the PAT as the password, then base64-encode the result.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/azure-devops-artifacts-api-openapi.yml
  - openapi/azure-devops-builds-api-openapi.yml
  - openapi/azure-devops-git-api-openapi.yml
  - openapi/azure-devops-pipelines-api-openapi.yml
  - openapi/azure-devops-releases-api-openapi.yml
  - openapi/azure-devops-service-hooks-api-openapi.yml
  - openapi/azure-devops-test-plans-api-openapi.yml
  - openapi/azure-devops-wiki-api-openapi.yml
  - openapi/azure-devops-work-items-api-openapi.yml
  type: http
slug: microsoft-azure-devops-authentication
source_filename: microsoft-azure-devops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-devops-artifacts-api-openapi.yml, openapi/azure-devops-builds-api-openapi.yml,\n  openapi/azure-devops-git-api-openapi.yml, openapi/azure-devops-pipelines-api-openapi.yml,\n  openapi/azure-devops-releases-api-openapi.yml, openapi/azure-devops-service-hooks-api-openapi.yml,\n  openapi/azure-devops-test-plans-api-openapi.yml, openapi/azure-devops-wiki-api-openapi.yml,\n  openapi/azure-devops-work-items-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Azure AD OAuth 2.0 bearer token\n  sources:\n  - openapi/azure-devops-artifacts-api-openapi.yml\n  - openapi/azure-devops-builds-api-openapi.yml\n  - openapi/azure-devops-git-api-openapi.yml\n  - openapi/azure-devops-pipelines-api-openapi.yml\n  - openapi/azure-devops-releases-api-openapi.yml\n  - openapi/azure-devops-service-hooks-api-openapi.yml\n  - openapi/azure-devops-test-plans-api-openapi.yml\n\
  \  - openapi/azure-devops-wiki-api-openapi.yml\n  - openapi/azure-devops-work-items-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication using a Personal Access Token (PAT). Use any string as the\n    username and the PAT as the password, then base64-encode the result.\n  sources:\n  - openapi/azure-devops-artifacts-api-openapi.yml\n  - openapi/azure-devops-builds-api-openapi.yml\n  - openapi/azure-devops-git-api-openapi.yml\n  - openapi/azure-devops-pipelines-api-openapi.yml\n  - openapi/azure-devops-releases-api-openapi.yml\n  - openapi/azure-devops-service-hooks-api-openapi.yml\n  - openapi/azure-devops-test-plans-api-openapi.yml\n  - openapi/azure-devops-wiki-api-openapi.yml\n  - openapi/azure-devops-work-items-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/authentication/microsoft-azure-devops-authentication.yml
summary_line: http · 2 schemes
tags:
- Agile
- CI/CD
- DevOps
- Project Management
- Version Control
---
