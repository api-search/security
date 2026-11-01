---
anonymous_access: false
api_key_in: []
api_specs:
- filename: granola-inbox-messages-api-openapi.yml
  format: yaml
  label: Granola Inbox Messages API
  slug: granola-inbox-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granola/openapi/granola-inbox-messages-api-openapi.yml
- filename: granola-inboxes-api-openapi.yml
  format: yaml
  label: Granola Inboxes API
  slug: granola-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granola/openapi/granola-inboxes-api-openapi.yml
- filename: granola-trigger-inbox-api-api-openapi.yml
  format: yaml
  label: Granola Trigger Inbox API
  slug: granola-trigger-inbox-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granola/openapi/granola-trigger-inbox-api-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Granola Authentication
name_suffix: Authentication
oauth_flows: []
overview: Granola secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Granola
provider_slug: granola
scheme_count: 1
schemes:
- bearerFormat: API key (grn_...)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/granola-openapi.yml
  type: http
slug: granola-authentication
source_filename: granola-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/granola-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key (grn_...)\n  sources:\n  - openapi/granola-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/granola/authentication/granola-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Meeting Notes
- Transcription
- Productivity
- MCP
- Zapier
- Business
- Enterprise
---
