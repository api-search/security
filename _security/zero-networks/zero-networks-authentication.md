---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: zero-networks-platform-openapi.yaml
  format: yaml
  label: Zero Networks Platform API
  slug: zero-networks-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-platform-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Zero Networks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zero Networks secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zero Networks
provider_slug: zero-networks
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/zero-networks-platform-openapi.yaml
  type: apiKey
slug: zero-networks-authentication
source_filename: zero-networks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/zero-networks-platform-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/zero-networks-platform-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/authentication/zero-networks-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Network Security
- Microsegmentation
- Zero Trust
- Identity
- Multi-Factor Authentication
- Segmentation
- ZTNA
- Kubernetes
- Cybersecurity
---
