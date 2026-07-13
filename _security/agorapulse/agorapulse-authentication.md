---
api_key_in:
- header
api_specs:
- filename: open-api.yml
  format: yaml
  label: Agorapulse Reports Open API
  slug: agorapulse-reports-api
  spec_type: OpenAPI
  url: https://api.agorapulse.com/docs/open-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Agorapulse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agorapulse secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agorapulse
provider_slug: agorapulse
scheme_count: 1
schemes:
- in: header
  name: bearerAuth
  parameter: X-API-KEY
  sources:
  - openapi/agorapulse-openapi.yml
  type: apiKey
slug: agorapulse-authentication
source_filename: agorapulse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agorapulse-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/agorapulse-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/authentication/agorapulse-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Social Media Management
- Social Media
- CRM
- Analytics
- Publishing
- Inbox Management
- Social Listening
---
