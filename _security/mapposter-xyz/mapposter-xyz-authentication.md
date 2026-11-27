---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mapposter-xyz-checkout-api-openapi.yml
  format: yaml
  label: MapPoster Checkout API
  slug: mapposter-xyz-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-checkout-api-openapi.yml
- filename: mapposter-xyz-health-api-openapi.yml
  format: yaml
  label: MapPoster Health API
  slug: mapposter-xyz-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-health-api-openapi.yml
- filename: mapposter-xyz-key-api-openapi.yml
  format: yaml
  label: MapPoster Key API
  slug: mapposter-xyz-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-key-api-openapi.yml
- filename: mapposter-xyz-keys-api-openapi.yml
  format: yaml
  label: MapPoster Keys API
  slug: mapposter-xyz-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-keys-api-openapi.yml
- filename: mapposter-xyz-me-api-openapi.yml
  format: yaml
  label: MapPoster Me API
  slug: mapposter-xyz-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-me-api-openapi.yml
- filename: mapposter-xyz-render-api-openapi.yml
  format: yaml
  label: MapPoster Render API
  slug: mapposter-xyz-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-render-api-openapi.yml
- filename: mapposter-xyz-verify-api-openapi.yml
  format: yaml
  label: MapPoster Verify API
  slug: mapposter-xyz-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapposter-xyz/openapi/mapposter-xyz-verify-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MapPoster Authentication
name_suffix: Authentication
oauth_flows: []
overview: MapPoster secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MapPoster
provider_slug: mapposter-xyz
scheme_count: 1
schemes:
- description: 'A Render API key (mpk_live_…): Starter, Pro, Business or Single Render, from https://mapposter.xyz/developers/ or POST /v1/checkout.'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/mapposter-xyz-openapi.json
  type: http
slug: mapposter-xyz-authentication
source_filename: mapposter-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/mapposter-xyz-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'A Render API key (mpk_live_…): Starter, Pro, Business or Single Render, from\n    https://mapposter.xyz/developers/ or POST /v1/checkout.'\n  sources:\n  - openapi/mapposter-xyz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mapposter-xyz/authentication/mapposter-xyz-authentication.yml
summary_line: http · 1 scheme
tags:
- Mapping
- Design
- E-Commerce
- AI Integration
- OpenStreetMap
---
