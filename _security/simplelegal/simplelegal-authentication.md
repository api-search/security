---
api_key_in: []
api_specs:
- filename: simplelegal-openapi.yml
  format: yaml
  label: SimpleLegal API
  slug: simplelegal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplelegal/refs/heads/main/openapi/simplelegal-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Simplelegal Authentication
name_suffix: Authentication
oauth_flows: []
overview: SimpleLegal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SimpleLegal
provider_slug: simplelegal
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using your SimpleLegal API credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/simplelegal-openapi.yml
  type: http
slug: simplelegal-authentication
source_filename: simplelegal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/simplelegal-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using your SimpleLegal API credentials.\n  sources:\n  - openapi/simplelegal-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplelegal/refs/heads/main/authentication/simplelegal-authentication.yml
summary_line: http · 1 scheme
tags:
- eBilling
- Enterprise Legal Management
- Legal Operations
- Legal Spend Management
- Matter Management
- Vendor Management
---
