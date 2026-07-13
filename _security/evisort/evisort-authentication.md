---
api_key_in: []
api_specs:
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Documents API
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Field and Metadata Extraction API
  slug: field-extraction
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Workflow API
  slug: workflows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Evisort Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evisort secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Evisort
provider_slug: evisort
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT bearer token obtained from POST /auth/token by presenting an Evisort API key.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/evisort-openapi.yml
  type: http
slug: evisort-authentication
source_filename: evisort-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/evisort-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer token obtained from POST /auth/token by presenting an Evisort API\n    key.\n  sources:\n  - openapi/evisort-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/authentication/evisort-authentication.yml
summary_line: http · 1 scheme
tags:
- Contract Lifecycle Management
- CLM
- Contract Intelligence
- Document AI
- Legal Tech
---
