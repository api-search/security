---
api_key_in:
- header
api_specs:
- filename: uipath-orchestrator-openapi.yml
  format: yaml
  label: UiPath Orchestrator API
  slug: uipath-orchestrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/openapi/uipath-orchestrator-openapi.yml
- filename: uipath-automation-hub-openapi.yml
  format: yaml
  label: UiPath Automation Hub API
  slug: uipath-automation-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/openapi/uipath-automation-hub-openapi.yml
- filename: uipath-document-understanding-openapi.yml
  format: yaml
  label: UiPath Document Understanding API
  slug: uipath-document-understanding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/openapi/uipath-document-understanding-openapi.yml
- filename: uipath-data-service-openapi.yml
  format: yaml
  label: UiPath Data Service API
  slug: uipath-data-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/openapi/uipath-data-service-openapi.yml
- filename: uipath-platform-management-openapi.yml
  format: yaml
  label: UiPath Platform Management API
  slug: uipath-platform-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/openapi/uipath-platform-management-openapi.yml
- filename: uipath-test-manager-openapi.yml
  format: yaml
  label: UiPath Test Manager API
  slug: uipath-test-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/openapi/uipath-test-manager-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Uipath Authentication
name_suffix: Authentication
oauth_flows: []
overview: UiPath secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: UiPath
provider_slug: uipath
scheme_count: 2
schemes:
- description: 'API token generated from the Automation Hub Admin Console under Platform Setup > Open API. Include as a Bearer token in the Authorization header: "Bearer {token}".'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/uipath-automation-hub-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token obtained from the UiPath Identity Server. Data Service scopes include DataService.Data and DataService.Data.Read. Tokens are valid for one hour; refresh tokens are supported.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/uipath-data-service-openapi.yml
  - openapi/uipath-document-understanding-openapi.yml
  - openapi/uipath-orchestrator-openapi.yml
  - openapi/uipath-platform-management-openapi.yml
  - openapi/uipath-test-manager-openapi.yml
  type: http
slug: uipath-authentication
source_filename: uipath-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uipath-automation-hub-openapi.yml, openapi/uipath-data-service-openapi.yml,\n  openapi/uipath-document-understanding-openapi.yml, openapi/uipath-orchestrator-openapi.yml,\n  openapi/uipath-platform-management-openapi.yml, openapi/uipath-test-manager-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API token generated from the Automation Hub Admin Console under Platform Setup\n    > Open API. Include as a Bearer token in the Authorization header: \"Bearer {token}\".'\n  sources:\n  - openapi/uipath-automation-hub-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token obtained from the UiPath Identity Server. Data Service\n    scopes include DataService.Data and DataService.Data.Read. Tokens are valid for one hour;\n\
  \    refresh tokens are supported.\n  sources:\n  - openapi/uipath-data-service-openapi.yml\n  - openapi/uipath-document-understanding-openapi.yml\n  - openapi/uipath-orchestrator-openapi.yml\n  - openapi/uipath-platform-management-openapi.yml\n  - openapi/uipath-test-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/authentication/uipath-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Automation
- Robotic Process Automation
- RPA
- Artificial Intelligence
- Document Processing
- Enterprise Automation
- Orchestration
- Testing
---
