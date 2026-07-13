---
api_key_in: []
api_specs:
- filename: talend-orchestration-openapi.yml
  format: yaml
  label: Talend Cloud Orchestration API
  slug: talend-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-orchestration-openapi.yml
- filename: talend-processing-openapi.yml
  format: yaml
  label: Talend Cloud Processing API
  slug: talend-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-processing-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Talend Authentication
name_suffix: Authentication
oauth_flows: []
overview: Talend secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Talend
provider_slug: talend
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token from Talend Cloud personal access token or service account token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/talend-orchestration-openapi.yml
  - openapi/talend-processing-openapi.yml
  type: http
slug: talend-authentication
source_filename: talend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/talend-orchestration-openapi.yml, openapi/talend-processing-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token from Talend Cloud personal access token or service account token\n  sources:\n  - openapi/talend-orchestration-openapi.yml\n  - openapi/talend-processing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/authentication/talend-authentication.yml
summary_line: http · 1 scheme
tags:
- API Management
- Data Integration
- Data Quality
- ETL
- Orchestration
- Pipelines
---
