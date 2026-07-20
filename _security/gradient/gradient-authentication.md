---
api_key_in: []
api_specs:
- filename: gradient-cloud-openapi.yml
  format: yaml
  label: Gradient Cloud AI API
  slug: gradient-cloud-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient/refs/heads/main/openapi/gradient-cloud-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Gradient Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gradient secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gradient
provider_slug: gradient
scheme_count: 1
schemes:
- description: 'Access Key passed as `Authorization: Bearer <access-key>`.'
  name: AccessKey
  scheme: bearer
  sources:
  - openapi/gradient-cloud-openapi.yml
  type: http
slug: gradient-authentication
source_filename: gradient-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/gradient-cloud-openapi.yml\ndocs: https://docs.gradient.network/enterprise-solutions/gradient-cloud/api-reference-documentation\nnotes: >-\n  Gradient Cloud uses Access Key authentication passed as an HTTP Bearer token\n  (`Authorization: Bearer <access-key>`). The List Models endpoint is public (no\n  auth). No OAuth or OpenID Connect surface is published; there is no scope model.\nsummary:\n  types:\n  - http\nschemes:\n- name: AccessKey\n  type: http\n  scheme: bearer\n  description: 'Access Key passed as `Authorization: Bearer <access-key>`.'\n  sources:\n  - openapi/gradient-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gradient/refs/heads/main/authentication/gradient-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Crypto Web3
- Artificial Intelligence
- Machine Learning
- LLM Inference
- Decentralized Infrastructure
- Distributed Computing
- Edge Computing
- Developer Tools
---
