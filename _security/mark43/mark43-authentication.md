---
api_key_in: []
api_specs:
- filename: mark43-partnerships-openapi.yml
  format: yaml
  label: Mark43 Partnerships API
  slug: mark43-partnerships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-partnerships-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mark43 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mark43 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mark43
provider_slug: mark43
scheme_count: 1
schemes:
- description: Secure API token presented via the standard HTTP Basic Authorization header on every request; issued by your Mark43 Technical Services Representative.
  name: httpBasic
  scheme: basic
  sources:
  - openapi/mark43-partnerships-openapi.yml
  type: http
slug: mark43-authentication
source_filename: mark43-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mark43-partnerships-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: httpBasic\n  type: http\n  scheme: basic\n  description: Secure API token presented via the standard HTTP Basic Authorization header on\n    every request; issued by your Mark43 Technical Services Representative.\n  sources:\n  - openapi/mark43-partnerships-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/authentication/mark43-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Public Safety
- Law Enforcement
- Records Management
- Computer-Aided Dispatch
- CAD
- RMS
- GovTech
- Evidence Management
- Government
---
