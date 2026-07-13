---
api_key_in:
- header
api_specs:
- filename: amazon-nova-openapi.yml
  format: yaml
  label: Amazon Nova API
  slug: amazon-nova-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-nova/refs/heads/main/openapi/amazon-nova-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Nova Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Nova secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Nova
provider_slug: amazon-nova
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed request.
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/amazon-nova-openapi.yml
  type: apiKey
slug: amazon-nova-authentication
source_filename: amazon-nova-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-nova-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed request.\n  sources:\n  - openapi/amazon-nova-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-nova/refs/heads/main/authentication/amazon-nova-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Foundation Models
- Generative AI
- Image Generation
- Machine Learning
- Multimodal
- Speech
- Video Generation
---
