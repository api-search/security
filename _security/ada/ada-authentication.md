---
api_key_in: []
api_specs:
- filename: ada-knowledge-openapi.yml
  format: yaml
  label: Ada Knowledge API
  slug: ada-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-knowledge-openapi.yml
- filename: ada-data-export-openapi.yml
  format: yaml
  label: Ada Data Export API
  slug: ada-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-data-export-openapi.yml
- filename: ada-data-compliance-openapi.yml
  format: yaml
  label: Ada Data Compliance API
  slug: ada-data-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-data-compliance-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ada Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ada secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ada
provider_slug: ada
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ada-data-compliance-openapi.yml
  - openapi/ada-data-export-openapi.yml
  - openapi/ada-data-export-v1-4-openapi.yml
  - openapi/ada-knowledge-openapi.yml
  type: http
slug: ada-authentication
source_filename: ada-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ada-data-compliance-openapi.yml, openapi/ada-data-export-openapi.yml, openapi/ada-data-export-v1-4-openapi.yml,\n  openapi/ada-knowledge-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ada-data-compliance-openapi.yml\n  - openapi/ada-data-export-openapi.yml\n  - openapi/ada-data-export-v1-4-openapi.yml\n  - openapi/ada-knowledge-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/authentication/ada-authentication.yml
summary_line: http · 1 scheme
tags:
- ai
- customer-service
- chatbot
- automation
- conversational-ai
- helpdesk
- crm
- integrations
- knowledge-management
- data-export
---
