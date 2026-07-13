---
api_key_in: []
api_specs:
- filename: drift-openapi.yml
  format: yaml
  label: Drift REST API
  slug: drift-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift/refs/heads/main/openapi/drift-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Drift Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drift secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Drift
provider_slug: drift
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/drift-openapi.yml
  type: http
slug: drift-authentication
source_filename: drift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drift-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/drift-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drift/refs/heads/main/authentication/drift-authentication.yml
summary_line: http · 1 scheme
tags:
- Conversational Marketing
- Chatbots
- Sales
- Messaging
- Customer Engagement
---
