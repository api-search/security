---
api_key_in:
- header
api_specs:
- filename: klaviyo-openapi.json
  format: json
  label: Klaviyo API
  slug: klaviyo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klaviyo/refs/heads/main/openapi/klaviyo-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Klaviyo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Klaviyo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Klaviyo
provider_slug: klaviyo
scheme_count: 1
schemes:
- description: Private key authentication for /api/ endpoints is performed by setting the `Authorization` header to `Klaviyo-API-Key your-private-api-key`<br>For more information please visit https://developers.klaviyo.com/en/v2026-04-15/reference/api-overview#authentication
  in: header
  name: Klaviyo-API-Key
  parameter: Authorization
  sources:
  - openapi/klaviyo-openapi.json
  type: apiKey
slug: klaviyo-authentication
source_filename: klaviyo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/klaviyo-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Klaviyo-API-Key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Private key authentication for /api/ endpoints is performed by setting the `Authorization`\n    header to `Klaviyo-API-Key your-private-api-key`<br>For more information please visit https://developers.klaviyo.com/en/v2026-04-15/reference/api-overview#authentication\n  sources:\n  - openapi/klaviyo-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klaviyo/refs/heads/main/authentication/klaviyo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Marketing
- Email
- SMS
- Customer Data
- Ecommerce
- Automation
---
