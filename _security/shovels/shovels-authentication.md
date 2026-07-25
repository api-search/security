---
api_key_in:
- header
api_specs:
- filename: shovels-addresses-api-openapi.yml
  format: yaml
  label: Shovels Addresses API
  slug: shovels-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shovels/refs/heads/main/openapi/shovels-addresses-api-openapi.yml
- filename: shovels-contractors-api-openapi.yml
  format: yaml
  label: Shovels Contractors API
  slug: shovels-contractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shovels/refs/heads/main/openapi/shovels-contractors-api-openapi.yml
- filename: shovels-geography-api-openapi.yml
  format: yaml
  label: Shovels Geography API
  slug: shovels-geography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shovels/refs/heads/main/openapi/shovels-geography-api-openapi.yml
- filename: shovels-lists-api-openapi.yml
  format: yaml
  label: Shovels Lists API
  slug: shovels-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shovels/refs/heads/main/openapi/shovels-lists-api-openapi.yml
- filename: shovels-meta-api-openapi.yml
  format: yaml
  label: Shovels Meta API
  slug: shovels-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shovels/refs/heads/main/openapi/shovels-meta-api-openapi.yml
- filename: shovels-permits-api-openapi.yml
  format: yaml
  label: Shovels Permits API
  slug: shovels-permits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shovels/refs/heads/main/openapi/shovels-permits-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shovels Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shovels secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shovels
provider_slug: shovels
scheme_count: 1
schemes:
- description: API key obtained from app.shovels.ai Profile Settings
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/shovels-openapi.yml
  type: apiKey
slug: shovels-authentication
source_filename: shovels-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shovels-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key obtained from app.shovels.ai Profile Settings\n  sources:\n  - openapi/shovels-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shovels/refs/heads/main/authentication/shovels-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Construction
- Building Permits
- Contractors
- Real Estate
- Property Data
- Market Intelligence
---
