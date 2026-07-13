---
api_key_in:
- header
api_specs:
- filename: slice-public-api-v1-openapi.yml
  format: yaml
  label: Slice Public API (v1)
  slug: rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slice/refs/heads/main/openapi/slice-public-api-v1-openapi.yml
- filename: slice-public-api-v2-openapi.yml
  format: yaml
  label: Slice Public API (v2)
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slice/refs/heads/main/openapi/slice-public-api-v2-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Slice Authentication
name_suffix: Authentication
oauth_flows: []
overview: Slice secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Slice
provider_slug: slice
scheme_count: 1
schemes:
- description: 'API key issued by Slice to approved technology partners. Request credentials

    from api-support@slicelife.com. The exact header name is assigned with the

    credentials; `Authorization` is used here as the documented placeholder.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/slice-public-api-v1-openapi.yml
  - openapi/slice-public-api-v2-openapi.yml
  type: apiKey
slug: slice-authentication
source_filename: slice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/slice-public-api-v1-openapi.yml, openapi/slice-public-api-v2-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    API key issued by Slice to approved technology partners. Request credentials\n    from api-support@slicelife.com. The exact header name is assigned with the\n    credentials; `Authorization` is used here as the documented placeholder.\n  sources:\n  - openapi/slice-public-api-v1-openapi.yml\n  - openapi/slice-public-api-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slice/refs/heads/main/authentication/slice-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- Pizza
- Online Ordering
- Local Commerce
- Menus
- Orders
---
