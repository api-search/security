---
api_key_in:
- header
api_specs:
- filename: crunchbase-openapi.yml
  format: yaml
  label: Crunchbase API
  slug: crunchbase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase/refs/heads/main/openapi/crunchbase-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Crunchbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crunchbase secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crunchbase
provider_slug: crunchbase
scheme_count: 1
schemes:
- description: Crunchbase user API key.
  in: header
  name: ApiKeyAuth
  parameter: X-cb-user-key
  sources:
  - openapi/crunchbase-openapi.yml
  type: apiKey
slug: crunchbase-authentication
source_filename: crunchbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/crunchbase-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-cb-user-key\n  description: Crunchbase user API key.\n  sources:\n  - openapi/crunchbase-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crunchbase/refs/heads/main/authentication/crunchbase-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Business Data
- Funding
- Investments
- Startups
- Private Markets
- Firmographics
---
