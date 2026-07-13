---
api_key_in:
- header
api_specs:
- filename: amazon-detective-openapi.yml
  format: yaml
  label: Amazon Detective API
  slug: amazon-detective-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/openapi/amazon-detective-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Detective Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Detective secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Detective
provider_slug: amazon-detective
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-detective-openapi.yml
  type: apiKey
slug: amazon-detective-authentication
source_filename: amazon-detective-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-detective-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-detective-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/authentication/amazon-detective-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Forensics
- Investigation
- Security
---
