---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-azure-pipelines-artifacts-api-openapi.yml
  format: yaml
  label: Azure Pipelines Artifacts API
  slug: microsoft-azure-pipelines-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-pipelines/openapi/microsoft-azure-pipelines-artifacts-api-openapi.yml
- filename: microsoft-azure-pipelines-build-artifacts-api-openapi.yml
  format: yaml
  label: Azure Pipelines Build Artifacts API
  slug: microsoft-azure-pipelines-build-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-pipelines/openapi/microsoft-azure-pipelines-build-artifacts-api-openapi.yml
- filename: microsoft-azure-pipelines-build-definitions-api-openapi.yml
  format: yaml
  label: Azure Pipelines Build Definitions API
  slug: microsoft-azure-pipelines-build-definitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-pipelines/openapi/microsoft-azure-pipelines-build-definitions-api-openapi.yml
- filename: microsoft-azure-pipelines-build-tags-api-openapi.yml
  format: yaml
  label: Azure Pipelines Build Tags API
  slug: microsoft-azure-pipelines-build-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-pipelines/openapi/microsoft-azure-pipelines-build-tags-api-openapi.yml
- filename: microsoft-azure-pipelines-builds-api-openapi.yml
  format: yaml
  label: Azure Pipelines Builds API
  slug: microsoft-azure-pipelines-builds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-pipelines/openapi/microsoft-azure-pipelines-builds-api-openapi.yml
- filename: microsoft-azure-pipelines-logs-api-openapi.yml
  format: yaml
  label: Azure Pipelines Logs API
  slug: microsoft-azure-pipelines-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-pipelines/openapi/microsoft-azure-pipelines-logs-api-openapi.yml
- filename: microsoft-azure-pipelines-pipelines-api-openapi.yml
  format: yaml
  label: Azure Pipelines API
  slug: microsoft-azure-pipelines-pipelines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-pipelines/openapi/microsoft-azure-pipelines-pipelines-api-openapi.yml
- filename: microsoft-azure-pipelines-runs-api-openapi.yml
  format: yaml
  label: Azure Pipelines Runs API
  slug: microsoft-azure-pipelines-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-pipelines/openapi/microsoft-azure-pipelines-runs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Microsoft Azure Pipelines Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure Pipelines secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Azure Pipelines
provider_slug: microsoft-azure-pipelines
scheme_count: 2
schemes:
- description: Azure AD OAuth 2.0 bearer token obtained through the authorization code flow with scope vso.build
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-azure-pipelines-artifacts-api-openapi.yml
  - openapi/microsoft-azure-pipelines-build-artifacts-api-openapi.yml
  - openapi/microsoft-azure-pipelines-build-definitions-api-openapi.yml
  - openapi/microsoft-azure-pipelines-build-tags-api-openapi.yml
  - openapi/microsoft-azure-pipelines-builds-api-openapi.yml
  - openapi/microsoft-azure-pipelines-logs-api-openapi.yml
  - openapi/microsoft-azure-pipelines-pipelines-api-openapi.yml
  - openapi/microsoft-azure-pipelines-runs-api-openapi.yml
  type: http
- description: Basic authentication using a Personal Access Token (PAT). Use any string as the username and the PAT as the password, then base64-encode the result.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/microsoft-azure-pipelines-artifacts-api-openapi.yml
  - openapi/microsoft-azure-pipelines-build-artifacts-api-openapi.yml
  - openapi/microsoft-azure-pipelines-build-definitions-api-openapi.yml
  - openapi/microsoft-azure-pipelines-build-tags-api-openapi.yml
  - openapi/microsoft-azure-pipelines-builds-api-openapi.yml
  - openapi/microsoft-azure-pipelines-logs-api-openapi.yml
  - openapi/microsoft-azure-pipelines-pipelines-api-openapi.yml
  - openapi/microsoft-azure-pipelines-runs-api-openapi.yml
  type: http
slug: microsoft-azure-pipelines-authentication
source_filename: microsoft-azure-pipelines-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/microsoft-azure-pipelines-artifacts-api-openapi.yml, openapi/microsoft-azure-pipelines-build-artifacts-api-openapi.yml,\n  openapi/microsoft-azure-pipelines-build-definitions-api-openapi.yml, openapi/microsoft-azure-pipelines-build-tags-api-openapi.yml,\n  openapi/microsoft-azure-pipelines-builds-api-openapi.yml, openapi/microsoft-azure-pipelines-logs-api-openapi.yml,\n  openapi/microsoft-azure-pipelines-pipelines-api-openapi.yml, openapi/microsoft-azure-pipelines-runs-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Azure AD OAuth 2.0 bearer token obtained through the authorization code flow\n    with scope vso.build\n  sources:\n  - openapi/microsoft-azure-pipelines-artifacts-api-openapi.yml\n  - openapi/microsoft-azure-pipelines-build-artifacts-api-openapi.yml\n  - openapi/microsoft-azure-pipelines-build-definitions-api-openapi.yml\n  - openapi/microsoft-azure-pipelines-build-tags-api-openapi.yml\n\
  \  - openapi/microsoft-azure-pipelines-builds-api-openapi.yml\n  - openapi/microsoft-azure-pipelines-logs-api-openapi.yml\n  - openapi/microsoft-azure-pipelines-pipelines-api-openapi.yml\n  - openapi/microsoft-azure-pipelines-runs-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication using a Personal Access Token (PAT). Use any string as the\n    username and the PAT as the password, then base64-encode the result.\n  sources:\n  - openapi/microsoft-azure-pipelines-artifacts-api-openapi.yml\n  - openapi/microsoft-azure-pipelines-build-artifacts-api-openapi.yml\n  - openapi/microsoft-azure-pipelines-build-definitions-api-openapi.yml\n  - openapi/microsoft-azure-pipelines-build-tags-api-openapi.yml\n  - openapi/microsoft-azure-pipelines-builds-api-openapi.yml\n  - openapi/microsoft-azure-pipelines-logs-api-openapi.yml\n  - openapi/microsoft-azure-pipelines-pipelines-api-openapi.yml\n  - openapi/microsoft-azure-pipelines-runs-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-pipelines/authentication/microsoft-azure-pipelines-authentication.yml
summary_line: http · 2 schemes
tags:
- Automation
- Builds
- CI/CD
- Deployment
- DevOps
- Pipelines
---
