---
api_key_in: []
api_specs:
- filename: lambda-cloud-api-openapi.yml
  format: yaml
  label: Lambda Cloud API
  slug: cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda/refs/heads/main/openapi/lambda-cloud-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lambda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lambda secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lambda
provider_slug: lambda
scheme_count: 1
schemes:
- description: Use your Lambda Cloud API key as the username with no password. Pass via Authorization header as Basic auth.
  name: apiKey
  scheme: basic
  sources:
  - openapi/lambda-cloud-api-openapi.yml
  type: http
slug: lambda-authentication
source_filename: lambda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lambda-cloud-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: basic\n  description: Use your Lambda Cloud API key as the username with no password. Pass via Authorization\n    header as Basic auth.\n  sources:\n  - openapi/lambda-cloud-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lambda/refs/heads/main/authentication/lambda-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Cloud Computing
- Compute
- Deep Learning
- GPU
- Machine Learning
---
