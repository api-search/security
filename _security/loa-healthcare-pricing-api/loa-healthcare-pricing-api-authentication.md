---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: loa-healthcare-pricing-api-entities-api-openapi.yml
  format: yaml
  label: Loa Healthcare Pricing API Entities API
  slug: loa-healthcare-pricing-api-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/openapi/loa-healthcare-pricing-api-entities-api-openapi.yml
- filename: loa-healthcare-pricing-api-entity-analytics-api-openapi.yml
  format: yaml
  label: Loa Healthcare Pricing API Entity Analytics API
  slug: loa-healthcare-pricing-api-entity-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/openapi/loa-healthcare-pricing-api-entity-analytics-api-openapi.yml
- filename: loa-healthcare-pricing-api-entity-updates-api-openapi.yml
  format: yaml
  label: Loa Healthcare Pricing API Entity Updates API
  slug: loa-healthcare-pricing-api-entity-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/openapi/loa-healthcare-pricing-api-entity-updates-api-openapi.yml
- filename: loa-healthcare-pricing-api-prices-api-openapi.yml
  format: yaml
  label: Loa Healthcare Pricing API Prices API
  slug: loa-healthcare-pricing-api-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/openapi/loa-healthcare-pricing-api-prices-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Loa Healthcare Pricing Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loa Healthcare Pricing API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Loa Healthcare Pricing API
provider_slug: loa-healthcare-pricing-api
scheme_count: 1
schemes:
- description: Optional provider API key for metered clients. Local public reads still work without a key.
  in: header
  name: ProviderApiKey
  parameter: x-api-key
  sources:
  - openapi/loa-healthcare-pricing-api-entities-api-openapi.yml
  - openapi/loa-healthcare-pricing-api-entity-analytics-api-openapi.yml
  - openapi/loa-healthcare-pricing-api-entity-updates-api-openapi.yml
  - openapi/loa-healthcare-pricing-api-prices-api-openapi.yml
  type: apiKey
slug: loa-healthcare-pricing-api-authentication
source_filename: loa-healthcare-pricing-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: derived\nsource: openapi/loa-healthcare-pricing-api-entities-api-openapi.yml, openapi/loa-healthcare-pricing-api-entity-analytics-api-openapi.yml,\n  openapi/loa-healthcare-pricing-api-entity-updates-api-openapi.yml, openapi/loa-healthcare-pricing-api-prices-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ProviderApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Optional provider API key for metered clients. Local public reads still work\n    without a key.\n  sources:\n  - openapi/loa-healthcare-pricing-api-entities-api-openapi.yml\n  - openapi/loa-healthcare-pricing-api-entity-analytics-api-openapi.yml\n  - openapi/loa-healthcare-pricing-api-entity-updates-api-openapi.yml\n  - openapi/loa-healthcare-pricing-api-prices-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/authentication/loa-healthcare-pricing-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Healthcare
- Price Transparency
- medical pricing
- Hospitals
- Providers
- Provider Directory
- hospital prices
- CPT
- HCPCS
- MCP
- agent-native
- OpenAPI
- llms-txt
---
