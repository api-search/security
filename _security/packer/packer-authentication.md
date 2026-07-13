---
api_key_in:
- header
api_specs:
- filename: packer-openapi.yml
  format: yaml
  label: Packer
  slug: packer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packer/refs/heads/main/openapi/packer-openapi.yml
- filename: packer-openapi.yml
  format: yaml
  label: HCP Packer Artifact Registry API
  slug: hcp-packer-artifact-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packer/refs/heads/main/openapi/packer-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Packer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Packer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Packer
provider_slug: packer
scheme_count: 1
schemes:
- description: 'Authentication token, prefixed by Bearer: Bearer <token>'
  in: header
  name: bearer
  parameter: Authorization
  sources:
  - openapi/packer-openapi.yml
  type: apiKey
slug: packer-authentication
source_filename: packer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/packer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Authentication token, prefixed by Bearer: Bearer <token>'\n  sources:\n  - openapi/packer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packer/refs/heads/main/authentication/packer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automation
- DevOps
- HashiCorp
- Image Building
- Infrastructure as Code
---
