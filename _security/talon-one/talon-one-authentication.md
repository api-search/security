---
api_key_in:
- header
api_specs:
- filename: talon-one-openapi.yml
  format: yaml
  label: Talon.One Integration API
  slug: talon-one-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-openapi.yml
- filename: talon-one-openapi.yml
  format: yaml
  label: Talon.One Management API
  slug: talon-one-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-openapi.yml
- filename: talon-one-openapi.yml
  format: yaml
  label: Talon.One Campaigns API
  slug: talon-one-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-openapi.yml
- filename: talon-one-openapi.yml
  format: yaml
  label: Talon.One Coupons API
  slug: talon-one-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-openapi.yml
- filename: talon-one-openapi.yml
  format: yaml
  label: Talon.One Loyalty API
  slug: talon-one-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Talon One Authentication
name_suffix: Authentication
oauth_flows: []
overview: Talon.One secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Talon.One
provider_slug: talon-one
scheme_count: 1
schemes:
- description: 'Integration API key with the ApiKey-v1 prefix, e.g. header "Authorization: ApiKey-v1 <your-key>".'
  in: header
  name: integrationKey
  parameter: Authorization
  sources:
  - openapi/talon-one-openapi.yml
  type: apiKey
slug: talon-one-authentication
source_filename: talon-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/talon-one-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: integrationKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Integration API key with the ApiKey-v1 prefix, e.g. header \"Authorization: ApiKey-v1\n    <your-key>\".'\n  sources:\n  - openapi/talon-one-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/authentication/talon-one-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Promotions
- Loyalty
- Coupons
- Incentives
- Campaigns
- Personalization
- MarTech
- Rules Engine
---
