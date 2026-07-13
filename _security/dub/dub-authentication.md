---
api_key_in: []
api_specs:
- filename: dub-openapi.yml
  format: yaml
  label: Dub Links API
  slug: links
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dub Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dub secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dub
provider_slug: dub
scheme_count: 1
schemes:
- description: Default authentication mechanism
  name: token
  scheme: bearer
  sources:
  - openapi/dub-openapi.yml
  type: http
slug: dub-authentication
source_filename: dub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dub-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: token\n  type: http\n  scheme: bearer\n  description: Default authentication mechanism\n  sources:\n  - openapi/dub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/authentication/dub-authentication.yml
summary_line: http · 1 scheme
tags:
- Link Management
- URL Shortener
- Analytics
- Conversion Tracking
- Affiliate Programs
- Open Source
---
