---
api_key_in: []
api_specs:
- filename: university-of-cambridge-lookup.yaml
  format: yaml
  label: Lookup / Ibis Web Service API
  slug: lookup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-cambridge/refs/heads/main/openapi/university-of-cambridge-lookup.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: University Of Cambridge Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Cambridge secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Cambridge
provider_slug: university-of-cambridge
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/university-of-cambridge-lookup.yaml
  type: http
slug: university-of-cambridge-authentication
source_filename: university-of-cambridge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-cambridge-lookup.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/university-of-cambridge-lookup.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-cambridge/refs/heads/main/authentication/university-of-cambridge-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- United Kingdom
- Identity
- API Gateway
- Developer Portal
---
