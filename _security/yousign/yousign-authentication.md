---
api_key_in: []
api_specs:
- filename: 6759d057a53fa9006fec9ff0
  format: yaml
  label: Yousign Public API v3
  slug: yousign-public-api-v3
  spec_type: OpenAPI
  url: https://developers.yousign.com/openapi/6759d057a53fa9006fec9ff0
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Yousign Authentication
name_suffix: Authentication
oauth_flows: []
overview: YouSign secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: YouSign
provider_slug: yousign
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/yousign-public-api-v3-openapi.yml
  type: http
slug: yousign-authentication
source_filename: yousign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/yousign-public-api-v3-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/yousign-public-api-v3-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yousign/refs/heads/main/authentication/yousign-authentication.yml
summary_line: http · 1 scheme
tags:
- E-Signature
- Electronic Signature
- eIDAS
- Digital Signature
- Document Signing
- Europe
- REST API
- Signature Workflows
---
