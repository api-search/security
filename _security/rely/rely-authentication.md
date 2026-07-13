---
api_key_in: []
api_specs:
- filename: rely-openapi.yml
  format: yaml
  label: Rely.io Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rely/refs/heads/main/openapi/rely-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rely Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rely.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rely.io
provider_slug: rely
scheme_count: 1
schemes:
- description: Long-lived API key generated in the Rely.io Plugins settings page. Valid for 10 years. Include as Bearer token in Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rely-openapi.yml
  type: http
slug: rely-authentication
source_filename: rely-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rely-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Long-lived API key generated in the Rely.io Plugins settings page. Valid for\n    10 years. Include as Bearer token in Authorization header.\n  sources:\n  - openapi/rely-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rely/refs/heads/main/authentication/rely-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer Experience
- Internal Developer Portal
- Platform Engineering
- Software Catalog
- Service Catalog
- Engineering Scorecards
---
