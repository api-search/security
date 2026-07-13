---
api_key_in: []
api_specs:
- filename: dnsimple-openapi.yml
  format: yaml
  label: DNSimple API
  slug: dnsimple
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dnsimple/refs/heads/main/openapi/dnsimple-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dnsimple Authentication
name_suffix: Authentication
oauth_flows: []
overview: DNSimple secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DNSimple
provider_slug: dnsimple
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dnsimple-openapi.yml
  type: http
slug: dnsimple-authentication
source_filename: dnsimple-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dnsimple-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/dnsimple-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dnsimple/refs/heads/main/authentication/dnsimple-authentication.yml
summary_line: http · 1 scheme
tags:
- DNS
- Domains
---
