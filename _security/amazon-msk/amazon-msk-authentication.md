---
api_key_in:
- header
api_specs:
- filename: amazon-msk-openapi-original.yml
  format: yaml
  label: Amazon MSK API
  slug: msk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/openapi/amazon-msk-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Msk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon MSK secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon MSK
provider_slug: amazon-msk
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-msk-openapi-original.yml
  type: apiKey
slug: amazon-msk-authentication
source_filename: amazon-msk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-msk-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-msk-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/authentication/amazon-msk-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Broadcasting
- Media Processing
- Media
---
