---
api_key_in:
- header
api_specs:
- filename: tapfiliate-rest-api-openapi.yml
  format: yaml
  label: Tapfiliate REST API
  slug: tapfiliate-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tapfiliate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tapfiliate secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tapfiliate
provider_slug: tapfiliate
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/tapfiliate-rest-api-openapi.yml
  type: apiKey
slug: tapfiliate-authentication
source_filename: tapfiliate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tapfiliate-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/tapfiliate-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/authentication/tapfiliate-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Affiliate Marketing
- Affiliate Tracking
- Commission Management
- Conversion Tracking
- Partner Programs
- Referral Programs
- Influencer Marketing
---
