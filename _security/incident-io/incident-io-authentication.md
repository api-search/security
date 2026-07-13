---
api_key_in: []
api_specs:
- filename: incident-io-openapi.yml
  format: yaml
  label: Incident.io
  slug: incident-io
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incident-io/refs/heads/main/openapi/incident-io-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Incident Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Incident.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Incident.io
provider_slug: incident-io
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/incident-io-openapi.yml
  type: http
slug: incident-io-authentication
source_filename: incident-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/incident-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/incident-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incident-io/refs/heads/main/authentication/incident-io-authentication.yml
summary_line: http · 1 scheme
tags:
- AIOps
- Incident Management
---
