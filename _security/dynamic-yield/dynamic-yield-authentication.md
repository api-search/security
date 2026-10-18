---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dynamic-yield-api-only-api-openapi.yml
  format: yaml
  label: Dynamic Yield API only API
  slug: dynamic-yield-api-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-api-only-api-openapi.yml
- filename: dynamic-yield-experience-apis-api-openapi.yml
  format: yaml
  label: Dynamic Yield Experience APIs API
  slug: dynamic-yield-experience-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-experience-apis-api-openapi.yml
- filename: dynamic-yield-product-data-api-openapi.yml
  format: yaml
  label: Dynamic Yield Product Data API
  slug: dynamic-yield-product-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-product-data-api-openapi.yml
- filename: dynamic-yield-profile-anywhere-api-openapi.yml
  format: yaml
  label: Dynamic Yield Profile Anywhere API
  slug: dynamic-yield-profile-anywhere-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-profile-anywhere-api-openapi.yml
- filename: dynamic-yield-user-data-api-api-openapi.yml
  format: yaml
  label: Dynamic Yield User Data API
  slug: dynamic-yield-user-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-user-data-api-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dynamic Yield Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dynamic Yield secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dynamic Yield
provider_slug: dynamic-yield
scheme_count: 1
schemes:
- description: Server-side Experience APIs authenticate with a Dynamic Yield API key passed in the DY-API-Key request header. API keys are section-scoped and generated in the Dynamic Yield admin console (Sections > API Keys). Distinct key types exist for server-side (Experience API) and other integration surfaces.
  docs: https://dy.dev/docs
  in: header
  name: DY-API-Key
  parameter: DY-API-Key
  type: apiKey
slug: dynamic-yield-authentication
source_filename: dynamic-yield-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://dy.dev/docs (Getting Started / API Keys) + https://dy.dev/reference\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: DY-API-Key\n  type: apiKey\n  in: header\n  parameter: DY-API-Key\n  description: >-\n    Server-side Experience APIs authenticate with a Dynamic Yield API key passed\n    in the DY-API-Key request header. API keys are section-scoped and generated\n    in the Dynamic Yield admin console (Sections > API Keys). Distinct key types\n    exist for server-side (Experience API) and other integration surfaces.\n  docs: https://dy.dev/docs\nnotes: >-\n  Client-side / script-based implementations are keyed by the section's public\n  data-dy-token snippet rather than the server-side DY-API-Key. No OpenAPI spec\n  was captured for this provider, so scheme details are sourced from the published\n  developer documentation rather than derived from a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/authentication/dynamic-yield-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cloud
- Personalization
- Experience Optimization
- Recommendations
- A/B Testing
- Search
- E-Commerce
- Retail
- Machine Learning
- MACH
- Mastercard
---
