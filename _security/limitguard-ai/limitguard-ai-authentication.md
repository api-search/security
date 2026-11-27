---
anonymous_access: false
api_key_in: []
api_specs:
- filename: limitguard-ai-entity-api-openapi.yml
  format: yaml
  label: Limitguard Entity API
  slug: limitguard-ai-entity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/limitguard-ai/openapi/limitguard-ai-entity-api-openapi.yml
- filename: limitguard-ai-risk-api-openapi.yml
  format: yaml
  label: Limitguard Risk API
  slug: limitguard-ai-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/limitguard-ai/openapi/limitguard-ai-risk-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Limitguard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Limitguard declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Limitguard
provider_slug: limitguard-ai
scheme_count: 1
schemes:
- description: Pass your API key in the X-API-Key header. Paid tier keys skip per-call payment.
  in: header
  name: X-API-Key
  type: apiKey
slug: limitguard-ai-authentication
source_filename: limitguard-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: searched\nsource: https://docs.limitguard.ai/authentication\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: Pass your API key in the X-API-Key header. Paid tier keys skip per-call payment.\n"
source_yaml_url: https://artifacts.apis.io/limitguard-ai/authentication/limitguard-ai-authentication.yml
summary_line: 1 scheme
tags:
- Lead Validation
- Data Verification
- Software-as-a-Service
- Europe
---
