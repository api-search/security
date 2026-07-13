---
api_key_in:
- header
api_specs:
- filename: amazon-q-business.json
  format: json
  label: Amazon Q Business API
  slug: amazon-q-business-api
  spec_type: OpenAPI
  url: https://example.com/openapi/amazon-q-business.json
- filename: amazon-q-developer.json
  format: json
  label: Amazon Q Developer API
  slug: amazon-q-developer-api
  spec_type: OpenAPI
  url: https://example.com/openapi/amazon-q-developer.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Q Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Q secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Q
provider_slug: amazon-q
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-q-openapi.yml
  type: apiKey
slug: amazon-q-authentication
source_filename: amazon-q-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-q-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-q-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/authentication/amazon-q-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Assistant
- Enterprise
- Generative AI
---
