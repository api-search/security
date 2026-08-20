---
api_key_in:
- header
api_specs:
- filename: conxai-annotations-api-openapi.yml
  format: yaml
  label: Conxai annotations API
  slug: conxai-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-annotations-api-openapi.yml
- filename: conxai-camera-api-openapi.yml
  format: yaml
  label: Conxai camera API
  slug: conxai-camera-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-camera-api-openapi.yml
- filename: conxai-document-types-api-openapi.yml
  format: yaml
  label: Conxai document-types API
  slug: conxai-document-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-document-types-api-openapi.yml
- filename: conxai-documents-api-openapi.yml
  format: yaml
  label: Conxai documents API
  slug: conxai-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-documents-api-openapi.yml
- filename: conxai-exports-api-openapi.yml
  format: yaml
  label: Conxai exports API
  slug: conxai-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-exports-api-openapi.yml
- filename: conxai-images-api-openapi.yml
  format: yaml
  label: Conxai Images API
  slug: conxai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-images-api-openapi.yml
- filename: conxai-integrations-api-openapi.yml
  format: yaml
  label: Conxai integrations API
  slug: conxai-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-integrations-api-openapi.yml
- filename: conxai-production-tracking-api-openapi.yml
  format: yaml
  label: Conxai production_tracking API
  slug: conxai-production-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-production-tracking-api-openapi.yml
- filename: conxai-project-api-openapi.yml
  format: yaml
  label: Conxai project API
  slug: conxai-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-project-api-openapi.yml
- filename: conxai-projects-api-openapi.yml
  format: yaml
  label: Conxai projects API
  slug: conxai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-projects-api-openapi.yml
- filename: conxai-samples-api-openapi.yml
  format: yaml
  label: Conxai samples API
  slug: conxai-samples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-samples-api-openapi.yml
- filename: conxai-schema-api-openapi.yml
  format: yaml
  label: Conxai schema API
  slug: conxai-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-schema-api-openapi.yml
- filename: conxai-summary-table-api-openapi.yml
  format: yaml
  label: Conxai summary-table API
  slug: conxai-summary-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-summary-table-api-openapi.yml
- filename: conxai-use-cases-api-openapi.yml
  format: yaml
  label: Conxai use-cases API
  slug: conxai-use-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-use-cases-api-openapi.yml
- filename: conxai-users-api-openapi.yml
  format: yaml
  label: Conxai users API
  slug: conxai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-users-api-openapi.yml
- filename: conxai-workflow-api-openapi.yml
  format: yaml
  label: Conxai workflow API
  slug: conxai-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-workflow-api-openapi.yml
- filename: conxai-workflow-table-api-openapi.yml
  format: yaml
  label: Conxai workflow-table API
  slug: conxai-workflow-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-workflow-table-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Conxai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conxai secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Conxai
provider_slug: conxai
scheme_count: 3
schemes:
- description: Provide the given API key
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/conxai-customer-openapi.json
  - openapi/conxai-docnostic-openapi.json
  - openapi/conxai-firestop-openapi.json
  type: apiKey
- description: Provide the JWT token in the Authorization header prefixed with "Bearer"
  in: header
  name: BearerAuth
  parameter: Authorization
  sources:
  - openapi/conxai-docnostic-openapi.json
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/conxai-production-tracking-openapi.json
  type: apiKey
slug: conxai-authentication
source_filename: conxai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/conxai-customer-openapi.json, openapi/conxai-docnostic-openapi.json, openapi/conxai-firestop-openapi.json,\n  openapi/conxai-production-tracking-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Provide the given API key\n  sources:\n  - openapi/conxai-customer-openapi.json\n  - openapi/conxai-docnostic-openapi.json\n  - openapi/conxai-firestop-openapi.json\n- name: BearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Provide the JWT token in the Authorization header prefixed with \"Bearer\"\n  sources:\n  - openapi/conxai-docnostic-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/conxai-production-tracking-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/authentication/conxai-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Construction
- AEC
- Artificial Intelligence
- Document Processing
- Computer-Vision
- Agentic AI
- Machine-Learning
---
