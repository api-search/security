---
api_key_in:
- header
api_specs:
- filename: amazon-mediatailor-openapi-original.yml
  format: yaml
  label: Amazon MediaTailor API
  slug: mediatailor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Mediatailor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon MediaTailor secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-mediatailor-openapi-original.yml
  type: apiKey
slug: amazon-mediatailor-authentication
source_filename: amazon-mediatailor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-mediatailor-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-mediatailor-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/authentication/amazon-mediatailor-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Broadcasting
- Media Processing
- Media
---
