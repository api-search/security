---
api_key_in: []
api_specs:
- filename: lambda-file-systems-api-openapi.yml
  format: yaml
  label: Lambda File Systems API
  slug: lambda-file-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda/refs/heads/main/openapi/lambda-file-systems-api-openapi.yml
- filename: lambda-images-api-openapi.yml
  format: yaml
  label: Lambda Images API
  slug: lambda-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda/refs/heads/main/openapi/lambda-images-api-openapi.yml
- filename: lambda-instance-types-api-openapi.yml
  format: yaml
  label: Lambda Instance Types API
  slug: lambda-instance-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda/refs/heads/main/openapi/lambda-instance-types-api-openapi.yml
- filename: lambda-instances-api-openapi.yml
  format: yaml
  label: Lambda Instances API
  slug: lambda-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda/refs/heads/main/openapi/lambda-instances-api-openapi.yml
- filename: lambda-ssh-keys-api-openapi.yml
  format: yaml
  label: Lambda SSH Keys API
  slug: lambda-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda/refs/heads/main/openapi/lambda-ssh-keys-api-openapi.yml
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
- Machine-Learning
---
