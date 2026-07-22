---
api_key_in:
- header
api_specs:
- filename: trustlayer-platform-v2-openapi.yaml
  format: yaml
  label: TrustLayer Platform API v2
  slug: trustlayer-platform-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustlayer/refs/heads/main/openapi/trustlayer-platform-v2-openapi.yaml
- filename: trustlayer-platform-v1-openapi.yaml
  format: yaml
  label: TrustLayer Platform API v1
  slug: trustlayer-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustlayer/refs/heads/main/openapi/trustlayer-platform-v1-openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trustlayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrustLayer secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TrustLayer
provider_slug: trustlayer
scheme_count: 2
schemes:
- in: header
  name: Token
  parameter: Authorization
  sources:
  - openapi/trustlayer-platform-v1-openapi.yaml
  type: apiKey
- description: 'Enter your API token:'
  name: Bearer Auth
  scheme: bearer
  sources:
  - openapi/trustlayer-platform-v2-openapi.yaml
  type: http
slug: trustlayer-authentication
source_filename: trustlayer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/trustlayer-platform-v1-openapi.yaml, openapi/trustlayer-platform-v2-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/trustlayer-platform-v1-openapi.yaml\n- name: Bearer Auth\n  type: http\n  scheme: bearer\n  description: 'Enter your API token:'\n  sources:\n  - openapi/trustlayer-platform-v2-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustlayer/refs/heads/main/authentication/trustlayer-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Fintech
- Insurtech
- Insurance
- Risk Management
- Compliance
- Certificate of Insurance
- Vendor Management
---
