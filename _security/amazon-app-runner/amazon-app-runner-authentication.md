---
api_key_in:
- header
api_specs:
- filename: amazon-app-runner-openapi.yaml
  format: yaml
  label: Amazon App Runner API
  slug: amazon-app-runner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/openapi/amazon-app-runner-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon App Runner Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon App Runner secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-app-runner-openapi.json
  - openapi/amazon-app-runner-openapi.yaml
  - openapi/amazon-app-runner-openapi.yml
  type: apiKey
slug: amazon-app-runner-authentication
source_filename: amazon-app-runner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-app-runner-openapi.json, openapi/amazon-app-runner-openapi.yaml, openapi/amazon-app-runner-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-app-runner-openapi.json\n  - openapi/amazon-app-runner-openapi.yaml\n  - openapi/amazon-app-runner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/authentication/amazon-app-runner-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
---
