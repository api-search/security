---
api_key_in:
- header
api_specs:
- filename: bloom-credit-api-openapi.yaml
  format: yaml
  label: Bloom Credit API
  slug: bloom-credit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloom-credit/refs/heads/main/openapi/bloom-credit-api-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bloom Credit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bloom Credit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bloom Credit
provider_slug: bloom-credit
scheme_count: 1
schemes:
- description: API key obtained from the Bloom Credit developer portal
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/bloom-credit-api-openapi.yaml
  type: apiKey
slug: bloom-credit-authentication
source_filename: bloom-credit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bloom-credit-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key obtained from the Bloom Credit developer portal\n  sources:\n  - openapi/bloom-credit-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloom-credit/refs/heads/main/authentication/bloom-credit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Credit Bureau
- Credit Reports
- Credit Scores
- Fintech
- Lending
- Personal Finance
---
