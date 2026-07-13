---
api_key_in:
- header
api_specs:
- filename: blissfully-vendr-catalog-api-openapi.yaml
  format: yaml
  label: Vendr Catalog API
  slug: vendr-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blissfully/refs/heads/main/openapi/blissfully-vendr-catalog-api-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Blissfully Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blissfully secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blissfully
provider_slug: blissfully
scheme_count: 1
schemes:
- description: API key for authentication. Contact Vendr support to obtain API access. Rate limited to 250 requests per minute and 150,000 per day.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/blissfully-vendr-catalog-api-openapi.yaml
  type: apiKey
slug: blissfully-authentication
source_filename: blissfully-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blissfully-vendr-catalog-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authentication. Contact Vendr support to obtain API access. Rate\n    limited to 250 requests per minute and 150,000 per day.\n  sources:\n  - openapi/blissfully-vendr-catalog-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blissfully/refs/heads/main/authentication/blissfully-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Procurement
- SaaS Discovery
- SaaS Management
- Software Procurement
- Spend Optimization
- Vendor Management
---
