---
api_key_in:
- header
api_specs:
- filename: amazon-inspector-openapi-original.yml
  format: yaml
  label: AWS Amazon Inspector API
  slug: aws-inspector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/openapi/amazon-inspector-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Inspector Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Inspector secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Inspector
provider_slug: amazon-inspector
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-inspector-openapi-original.yml
  - openapi/amazon-inspector-openapi.yml
  type: apiKey
slug: amazon-inspector-authentication
source_filename: amazon-inspector-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-inspector-openapi-original.yml, openapi/amazon-inspector-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-inspector-openapi-original.yml\n  - openapi/amazon-inspector-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/authentication/amazon-inspector-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
---
