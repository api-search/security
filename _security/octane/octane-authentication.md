---
api_key_in: []
api_specs:
- filename: openapi
  format: yaml
  label: Octane REST API
  slug: octane-rest-api
  spec_type: OpenAPI
  url: https://docs.getoctane.io/openapi
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Octane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Octane secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Octane
provider_slug: octane
scheme_count: 1
schemes:
- description: API key passed as a Bearer token in the Authorization header.
  name: BearerApiKeyAuth
  scheme: bearer
  sources:
  - openapi/octane-octane-rest-api-openapi.yml
  type: http
slug: octane-authentication
source_filename: octane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/octane-octane-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerApiKeyAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/octane-octane-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/authentication/octane-authentication.yml
summary_line: http · 1 scheme
tags:
- Usage-Based Billing
- Metered Billing
- Pricing Plans
- SaaS Monetization
- FinTech
- Payments
- Usage Tracking
- Meters
- Entitlements
---
