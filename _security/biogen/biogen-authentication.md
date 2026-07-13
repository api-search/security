---
api_key_in:
- header
api_specs:
- filename: biogen-developer-api-openapi.yml
  format: yaml
  label: Biogen Developer API
  slug: developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/openapi/biogen-developer-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Biogen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Biogen secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Biogen
provider_slug: biogen
scheme_count: 1
schemes:
- description: Biogen Developer API key passed in X-API-Key header
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/biogen-developer-api-openapi.yml
  type: apiKey
slug: biogen-authentication
source_filename: biogen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/biogen-developer-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Biogen Developer API key passed in X-API-Key header\n  sources:\n  - openapi/biogen-developer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/authentication/biogen-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Biotechnology
- Healthcare
- Life Sciences
- Pharmaceuticals
- Neurology
- Fortune 500
---
