---
api_key_in:
- header
api_specs:
- filename: harbor-compliance-openapi.yml
  format: yaml
  label: Harbor Compliance API
  slug: harbor-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/openapi/harbor-compliance-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Harbor Compliance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harbor Compliance secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Harbor Compliance
provider_slug: harbor-compliance
scheme_count: 1
schemes:
- description: API key for authenticating partner requests. Obtain your API key from the Harbor Compliance developer portal.
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/harbor-compliance-openapi.yml
  type: apiKey
slug: harbor-compliance-authentication
source_filename: harbor-compliance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/harbor-compliance-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authenticating partner requests. Obtain your API key from the Harbor\n    Compliance developer portal.\n  sources:\n  - openapi/harbor-compliance-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/authentication/harbor-compliance-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Business Licensing
- Compliance
- Legal
- Regulatory
---
