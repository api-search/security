---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: lotsmail-to-lotsmail-api-openapi.yml
  format: yaml
  label: LotsTech AI Solutions Private Limited Lots Mail API
  slug: lotsmail-to-lotsmail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lotsmail-to/openapi/lotsmail-to-lotsmail-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: LotsTech AI Solutions Private Limited Authentication
name_suffix: Authentication
oauth_flows: []
overview: LotsTech AI Solutions Private Limited secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LotsTech AI Solutions Private Limited
provider_slug: lotsmail-to
scheme_count: 1
schemes:
- description: 'API key for authentication. Format: REDACTED_STRIPE_KEY'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/lotsmail-to-openapi.json
  type: apiKey
slug: lotsmail-to-authentication
source_filename: lotsmail-to-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/lotsmail-to-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'API key for authentication. Format: REDACTED_STRIPE_KEY'\n  sources:\n  - openapi/lotsmail-to-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lotsmail-to/authentication/lotsmail-to-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email
- Business
- Software-as-a-Service
- Artificial Intelligence
- Communications
---
