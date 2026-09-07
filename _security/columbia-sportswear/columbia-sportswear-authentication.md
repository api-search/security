---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: columbia-sportswear-content-hub-external-openapi.json
  format: json
  label: Content Hub External API
  slug: content-hub-external
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/columbia-sportswear/refs/heads/main/openapi/columbia-sportswear-content-hub-external-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Columbia Sportswear Authentication
name_suffix: Authentication
oauth_flows: []
overview: Columbia Sportswear secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Columbia Sportswear
provider_slug: columbia-sportswear
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/columbia-sportswear-content-hub-external-openapi.json
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/columbia-sportswear-content-hub-external-openapi.json
  type: apiKey
slug: columbia-sportswear-authentication
source_filename: columbia-sportswear-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/columbia-sportswear-content-hub-external-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/columbia-sportswear-content-hub-external-openapi.json\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/columbia-sportswear-content-hub-external-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/columbia-sportswear/refs/heads/main/authentication/columbia-sportswear-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Apparel
- B2B
- Consumer Management
- Content Management
- Digital Asset Management
- Footwear
- Fortune 1000
- Outdoor
- Partner APIs
- Product Imagery
- Retail
---
