---
api_key_in: []
api_specs:
- filename: forethought-solve-api-openapi.yml
  format: yaml
  label: Forethought Solve API
  slug: forethought-solve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forethought/refs/heads/main/openapi/forethought-solve-api-openapi.yml
- filename: forethought-triage-api-openapi.yml
  format: yaml
  label: Forethought Triage API
  slug: forethought-triage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forethought/refs/heads/main/openapi/forethought-triage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Forethought Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forethought secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Forethought
provider_slug: forethought
scheme_count: 1
schemes:
- bearerFormat: Solve API token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/forethought-solve-api-openapi.yml
  - openapi/forethought-triage-api-openapi.yml
  type: http
slug: forethought-authentication
source_filename: forethought-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/forethought-solve-api-openapi.yml, openapi/forethought-triage-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Solve API token\n  sources:\n  - openapi/forethought-solve-api-openapi.yml\n  - openapi/forethought-triage-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forethought/refs/heads/main/authentication/forethought-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- Customer Support
- Customer Service
- Generative AI
- SupportGPT
- Conversational AI
- Ticket Triage
- Agentic AI
- Voice AI
- Helpdesk
- Multi-Agent
---
