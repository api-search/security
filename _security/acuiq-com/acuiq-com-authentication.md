---
anonymous_access: false
api_key_in: []
api_specs:
- filename: acuiq-com-checkout-api-openapi.yml
  format: yaml
  label: AcuiQ Checkout API
  slug: acuiq-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-checkout-api-openapi.yml
- filename: acuiq-com-corpus-api-openapi.yml
  format: yaml
  label: AcuiQ Corpus API
  slug: acuiq-com-corpus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-corpus-api-openapi.yml
- filename: acuiq-com-llms-txt-api-openapi.yml
  format: yaml
  label: AcuiQ Llms.txt API
  slug: acuiq-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-llms-txt-api-openapi.yml
- filename: acuiq-com-mcp-api-openapi.yml
  format: yaml
  label: AcuiQ MCP API
  slug: acuiq-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-mcp-api-openapi.yml
- filename: acuiq-com-meridians-api-openapi.yml
  format: yaml
  label: AcuiQ Meridians API
  slug: acuiq-com-meridians-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-meridians-api-openapi.yml
- filename: acuiq-com-protocols-api-openapi.yml
  format: yaml
  label: AcuiQ Protocols API
  slug: acuiq-com-protocols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-protocols-api-openapi.yml
- filename: acuiq-com-reviews-api-openapi.yml
  format: yaml
  label: AcuiQ Reviews API
  slug: acuiq-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-reviews-api-openapi.yml
- filename: acuiq-com-symptoms-api-openapi.yml
  format: yaml
  label: AcuiQ Symptoms API
  slug: acuiq-com-symptoms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-symptoms-api-openapi.yml
- filename: acuiq-com-wiki-api-openapi.yml
  format: yaml
  label: AcuiQ Wiki API
  slug: acuiq-com-wiki-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-wiki-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AcuiQ Authentication
name_suffix: Authentication
oauth_flows: []
overview: AcuiQ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AcuiQ
provider_slug: acuiq-com
scheme_count: 1
schemes:
- description: 'MPP (Machine Payments Protocol) (https://mpp.dev), method "stripe", paid with a Stripe shared payment token (SPT), single use scoped to Stripe profile profile_61VcHMvCI7idwYC2zA6VcHMv8oE9roGsBkZRtDHSi0ng. Request the resource without it, answer the WWW-Authenticate challenge from the 402, and retry with Authorization: Payment. Only the two bulk exports use this; everything else on this spec is fre'
  name: payment
  scheme: Payment
  sources:
  - openapi/acuiq-com-openapi.json
  type: http
slug: acuiq-com-authentication
source_filename: acuiq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/acuiq-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: payment\n  type: http\n  scheme: Payment\n  description: 'MPP (Machine Payments Protocol) (https://mpp.dev), method \"stripe\", paid with\n    a Stripe shared payment token (SPT), single use scoped to Stripe profile profile_61VcHMvCI7idwYC2zA6VcHMv8oE9roGsBkZRtDHSi0ng.\n    Request the resource without it, answer the WWW-Authenticate challenge from the 402, and\n    retry with Authorization: Payment. Only the two bulk exports use this; everything else on\n    this spec is fre'\n  sources:\n  - openapi/acuiq-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/acuiq-com/authentication/acuiq-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Health
- Acupuncture
- Data
- Research
- Wellness
---
