---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: viridisconservation-com-adoption-api-openapi.yml
  format: yaml
  label: viridisconservation-com Adoption API
  slug: viridisconservation-com-adoption-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-adoption-api-openapi.yml
- filename: viridisconservation-com-agents-api-openapi.yml
  format: yaml
  label: viridisconservation-com Agents API
  slug: viridisconservation-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-agents-api-openapi.yml
- filename: viridisconservation-com-climate-api-openapi.yml
  format: yaml
  label: viridisconservation-com Climate API
  slug: viridisconservation-com-climate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-climate-api-openapi.yml
- filename: viridisconservation-com-climate-compliance-api-openapi.yml
  format: yaml
  label: viridisconservation-com Climate Compliance API
  slug: viridisconservation-com-climate-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-climate-compliance-api-openapi.yml
- filename: viridisconservation-com-conservation-api-openapi.yml
  format: yaml
  label: viridisconservation-com Conservation API
  slug: viridisconservation-com-conservation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-conservation-api-openapi.yml
- filename: viridisconservation-com-construction-api-openapi.yml
  format: yaml
  label: viridisconservation-com Construction API
  slug: viridisconservation-com-construction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-construction-api-openapi.yml
- filename: viridisconservation-com-csrd-api-openapi.yml
  format: yaml
  label: viridisconservation-com Csrd API
  slug: viridisconservation-com-csrd-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-csrd-api-openapi.yml
- filename: viridisconservation-com-ghg-api-openapi.yml
  format: yaml
  label: viridisconservation-com Ghg API
  slug: viridisconservation-com-ghg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-ghg-api-openapi.yml
- filename: viridisconservation-com-routing-api-openapi.yml
  format: yaml
  label: viridisconservation-com Routing API
  slug: viridisconservation-com-routing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-routing-api-openapi.yml
- filename: viridisconservation-com-security-api-openapi.yml
  format: yaml
  label: viridisconservation-com Security API
  slug: viridisconservation-com-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-security-api-openapi.yml
- filename: viridisconservation-com-security-preflight-api-openapi.yml
  format: yaml
  label: viridisconservation-com Security Preflight API
  slug: viridisconservation-com-security-preflight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-security-preflight-api-openapi.yml
- filename: viridisconservation-com-tax-credit-api-openapi.yml
  format: yaml
  label: viridisconservation-com Tax Credit API
  slug: viridisconservation-com-tax-credit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-tax-credit-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Viridisconservation Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: viridisconservation-com secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: viridisconservation-com
provider_slug: viridisconservation-com
scheme_count: 1
schemes:
- description: Buyer-created x402 v2 payment signature supplied only after inspecting a fresh unpaid quote.
  in: header
  name: PaymentSignature
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/viridisconservation-com-openapi.json
  type: apiKey
slug: viridisconservation-com-authentication
source_filename: viridisconservation-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/viridisconservation-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: PaymentSignature\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: Buyer-created x402 v2 payment signature supplied only after inspecting a fresh\n    unpaid quote.\n  sources:\n  - openapi/viridisconservation-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/viridisconservation-com/authentication/viridisconservation-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Conservation
- Environment
- Data
- API
- SaaS
---
