---
api_key_in:
- header
api_specs:
- filename: amazon-amplify-openapi.yaml
  format: yaml
  label: Amazon Amplify REST API
  slug: amazon-amplify-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-amplify/refs/heads/main/openapi/amazon-amplify-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Amplify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Amplify secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Amplify
provider_slug: amazon-amplify
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-amplify-api-openapi.yml
  - openapi/amazon-amplify-openapi.yaml
  type: apiKey
slug: amazon-amplify-authentication
source_filename: amazon-amplify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-amplify-api-openapi.yml, openapi/amazon-amplify-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-amplify-api-openapi.yml\n  - openapi/amazon-amplify-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-amplify/refs/heads/main/authentication/amazon-amplify-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Frontend
- Full Stack
- Hosting
- Mobile Development
- Web Applications
---
