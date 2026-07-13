---
api_key_in: []
api_specs:
- filename: amazon-connect-openapi.yml
  format: yaml
  label: Amazon Connect Service API
  slug: amazon-connect-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Connect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Connect secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Connect
provider_slug: amazon-connect
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication. Requests must be signed using IAM credentials with appropriate Amazon Connect permissions.
  name: aws_signature
  scheme: bearer
  sources:
  - openapi/amazon-connect-openapi.yml
  type: http
slug: amazon-connect-authentication
source_filename: amazon-connect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-connect-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: aws_signature\n  type: http\n  scheme: bearer\n  description: AWS Signature Version 4 authentication. Requests must be signed using IAM credentials\n    with appropriate Amazon Connect permissions.\n  sources:\n  - openapi/amazon-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/authentication/amazon-connect-authentication.yml
summary_line: http · 1 scheme
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
---
