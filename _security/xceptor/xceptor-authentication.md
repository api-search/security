---
api_key_in: []
api_specs:
- filename: workflows
  format: yaml
  label: Xceptor Workflow API
  slug: xceptor-workflow-api
  spec_type: Postman
  url: https://www.postman.com/xceptor/workspace/workflows
- filename: xceptor-authentication-api-openapi.yml
  format: yaml
  label: Xceptor Authentication API
  slug: xceptor-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-authentication-api-openapi.yml
- filename: xceptor-data-sources-api-openapi.yml
  format: yaml
  label: Xceptor Data Sources API
  slug: xceptor-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-data-sources-api-openapi.yml
- filename: xceptor-documents-api-openapi.yml
  format: yaml
  label: Xceptor Documents API
  slug: xceptor-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-documents-api-openapi.yml
- filename: xceptor-extraction-api-openapi.yml
  format: yaml
  label: Xceptor Extraction API
  slug: xceptor-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-extraction-api-openapi.yml
- filename: xceptor-health-api-openapi.yml
  format: yaml
  label: Xceptor Health API
  slug: xceptor-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-health-api-openapi.yml
- filename: xceptor-jobs-api-openapi.yml
  format: yaml
  label: Xceptor Jobs API
  slug: xceptor-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-jobs-api-openapi.yml
- filename: xceptor-templates-api-openapi.yml
  format: yaml
  label: Xceptor Templates API
  slug: xceptor-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-templates-api-openapi.yml
- filename: xceptor-workflow-runs-api-openapi.yml
  format: yaml
  label: Xceptor Workflow Runs API
  slug: xceptor-workflow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-workflow-runs-api-openapi.yml
- filename: xceptor-workflow-steps-api-openapi.yml
  format: yaml
  label: Xceptor Workflow Steps API
  slug: xceptor-workflow-steps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-workflow-steps-api-openapi.yml
- filename: xceptor-workflows-api-openapi.yml
  format: yaml
  label: Xceptor Workflows API
  slug: xceptor-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-workflows-api-openapi.yml
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
- Financial-Services
- Intelligent Document Processing
- Reconciliations
- Trade Operations
---
