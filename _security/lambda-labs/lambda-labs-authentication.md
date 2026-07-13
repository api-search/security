---
api_key_in: []
api_specs:
- filename: lambda-labs-openapi.json
  format: json
  label: Lambda Cloud API
  slug: cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-openapi.json
- filename: lambda-labs-asyncapi.yml
  format: yaml
  label: Lambda Inference API
  slug: inference-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/asyncapi/lambda-labs-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lambda Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lambda secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lambda
provider_slug: lambda-labs
scheme_count: 2
schemes:
- description: 'Basic HTTP authentication. Allowed headers:

    * `Authorization: Basic <base64 encoding of api_key>:`

    * `Authorization: Basic <api_key>`'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/lambda-labs-openapi.json
  type: http
- description: 'Bearer HTTP authentication. Allowed headers:

    * `Authorization: Bearer <api_key>`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lambda-labs-openapi.json
  type: http
slug: lambda-labs-authentication
source_filename: lambda-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lambda-labs-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Basic HTTP authentication. Allowed headers:\n    * `Authorization: Basic <base64 encoding of api_key>:`\n    * `Authorization: Basic <api_key>`\n  sources:\n  - openapi/lambda-labs-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer HTTP authentication. Allowed headers:\n    * `Authorization: Bearer <api_key>`\n  sources:\n  - openapi/lambda-labs-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/authentication/lambda-labs-authentication.yml
summary_line: http · 2 schemes
tags:
- AI
- Cloud
- Clusters
- Compute
- GPU
- Inference
- Machine Learning
---
