---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Loops API
  slug: loops-api
  spec_type: OpenAPI
  url: https://app.loops.so/openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Loops So Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loops secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Loops
provider_slug: loops-so
scheme_count: 1
schemes:
- name: apiKey
  scheme: bearer
  sources:
  - openapi/loops-openapi.yml
  type: http
slug: loops-so-authentication
source_filename: loops-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/loops-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/loops-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/authentication/loops-so-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Marketing Email
- Transactional Email
- Email Automation
- Email Campaigns
- Email Workflows
- Contacts
- Audience Management
- Events
- Webhooks
- SaaS
- Developer Tools
---
