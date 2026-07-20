---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Xceptor REST API
  slug: xceptor-rest-api
  spec_type: OpenAPI
  url: https://api.xceptor.com/v1/openapi.json
- filename: workflows
  format: yaml
  label: Xceptor Workflow API
  slug: xceptor-workflow-api
  spec_type: Postman
  url: https://www.postman.com/xceptor/workspace/workflows
- filename: xceptor-document-upload-api-openapi.yml
  format: yaml
  label: Xceptor Document Upload API
  slug: xceptor-document-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-document-upload-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Xceptor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xceptor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Xceptor
provider_slug: xceptor
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth2 access token obtained via the client credentials flow. Include as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/xceptor-document-upload-api-openapi.yml
  - openapi/xceptor-rest-api-openapi.yml
  - openapi/xceptor-workflow-api-openapi.yml
  type: http
slug: xceptor-authentication
source_filename: xceptor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xceptor-document-upload-api-openapi.yml, openapi/xceptor-rest-api-openapi.yml,\n  openapi/xceptor-workflow-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 access token obtained via the client credentials flow. Include as a Bearer\n    token in the Authorization header.\n  sources:\n  - openapi/xceptor-document-upload-api-openapi.yml\n  - openapi/xceptor-rest-api-openapi.yml\n  - openapi/xceptor-workflow-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/authentication/xceptor-authentication.yml
summary_line: http · 1 scheme
tags:
- API Integration
- Data Automation
- Data Extraction
- Document Processing
- ETL
- Financial Data
- Financial Services
- Intelligent Document Processing
- Reconciliations
- Trade Operations
---
