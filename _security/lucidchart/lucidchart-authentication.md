---
api_key_in: []
api_specs:
- filename: lucidchart-openapi.yml
  format: yaml
  label: Lucid REST API
  slug: lucid-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidchart/refs/heads/main/openapi/lucidchart-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lucidchart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lucidchart secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lucidchart
provider_slug: lucidchart
scheme_count: 1
schemes:
- bearerFormat: OAuth 2.0 access token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lucidchart-openapi.yml
  type: http
slug: lucidchart-authentication
source_filename: lucidchart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lucidchart-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth 2.0 access token\n  sources:\n  - openapi/lucidchart-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucidchart/refs/heads/main/authentication/lucidchart-authentication.yml
summary_line: http · 1 scheme
tags:
- Productivity
- Diagramming
- Visualization
- Visual Workspace
- SaaS
---
