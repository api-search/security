---
api_key_in:
- header
api_specs:
- filename: lusha-account-api-openapi.yml
  format: yaml
  label: Lusha Account API
  slug: lusha-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-account-api-openapi.yml
- filename: lusha-enrichment-api-openapi.yml
  format: yaml
  label: Lusha Enrichment API
  slug: lusha-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-enrichment-api-openapi.yml
- filename: lusha-filters-api-openapi.yml
  format: yaml
  label: Lusha Filters API
  slug: lusha-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-filters-api-openapi.yml
- filename: lusha-lookalike-api-openapi.yml
  format: yaml
  label: Lusha Lookalike API
  slug: lusha-lookalike-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-lookalike-api-openapi.yml
- filename: lusha-prospecting-api-openapi.yml
  format: yaml
  label: Lusha Prospecting API
  slug: lusha-prospecting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-prospecting-api-openapi.yml
- filename: lusha-signals-api-openapi.yml
  format: yaml
  label: Lusha Signals API
  slug: lusha-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-signals-api-openapi.yml
- filename: lusha-webhooks-api-openapi.yml
  format: yaml
  label: Lusha Webhooks API
  slug: lusha-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lusha Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lusha secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lusha
provider_slug: lusha
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/lusha-openapi.yml
  type: apiKey
slug: lusha-authentication
source_filename: lusha-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lusha-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: api_key\n  sources:\n  - openapi/lusha-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/authentication/lusha-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sales Intelligence
- B2B
- Enrichment
- Contact Data
- Prospecting
- Intent
---
