---
api_key_in:
- header
api_specs:
- filename: replicated-vendor-api-v3-openapi-original.json
  format: json
  label: Replicated Vendor API v3
  slug: replicated-vendor-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicated/refs/heads/main/openapi/replicated-vendor-api-v3-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Replicated Authentication
name_suffix: Authentication
oauth_flows: []
overview: Replicated secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Replicated
provider_slug: replicated
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/replicated-vendor-api-v3-openapi-original.json
  type: apiKey
slug: replicated-authentication
source_filename: replicated-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/replicated-vendor-api-v3-openapi-original.json\ndocs: https://docs.replicated.com/vendor/replicated-api-tokens\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  token_types:\n  - user API token\n  - service account token\n  note: >-\n    Vendor API v3 uses a token in the Authorization header. Tokens are user API\n    tokens or service-account tokens created in the Vendor Portal; legacy Team API\n    tokens are deprecated. No OAuth flows, so there is no scope surface.\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/replicated-vendor-api-v3-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replicated/refs/heads/main/authentication/replicated-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Developer Tools
- Software Distribution
- Kubernetes
- On-Premises
- Application Delivery
- Air Gap
- Licensing
---
