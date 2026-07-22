---
api_key_in:
- header
api_specs:
- filename: oden-technologies-openapi-original.yml
  format: yaml
  label: Oden API v2
  slug: oden-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Oden Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oden Technologies secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oden Technologies
provider_slug: oden-technologies
scheme_count: 1
schemes:
- description: Prefix the value with \"Token\" to indicate the custom authorization type
  in: header
  name: APIKeyAuth
  parameter: Authorization
  sources:
  - openapi/oden-technologies-openapi-original.yml
  type: apiKey
slug: oden-technologies-authentication
source_filename: oden-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/oden-technologies-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Prefix the value with \\\"Token\\\" to indicate the custom authorization type\n  sources:\n  - openapi/oden-technologies-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/authentication/oden-technologies-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Manufacturing
- Industrial IoT
- Analytics
- Artificial Intelligence
- Factory
- Manufacturing Analytics
- API
---
