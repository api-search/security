---
api_key_in:
- header
api_specs:
- filename: trieve-openapi.yml
  format: yaml
  label: Trieve REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trieve/refs/heads/main/openapi/trieve-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trieve Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trieve secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trieve
provider_slug: trieve
scheme_count: 1
schemes:
- description: 'Trieve API key. User or API key must have admin or owner role on the

    targeted dataset''s organization.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/trieve-openapi.yml
  type: apiKey
slug: trieve-authentication
source_filename: trieve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trieve-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Trieve API key. User or API key must have admin or owner role on the\n    targeted dataset's organization.\n  sources:\n  - openapi/trieve-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trieve/refs/heads/main/authentication/trieve-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Search
- RAG
- Vector Search
- Hybrid Search
- Recommendations
- Analytics
- Open Source
---
