---
anonymous_access: false
api_key_in: []
api_specs:
- filename: simplevoip-call-recordings-api-openapi.yml
  format: yaml
  label: SimpleVoIP Call Recordings API
  slug: simplevoip-call-recordings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-call-recordings-api-openapi.yml
- filename: simplevoip-cdr-api-openapi.yml
  format: yaml
  label: SimpleVoIP CDR API
  slug: simplevoip-cdr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-cdr-api-openapi.yml
- filename: simplevoip-music-on-hold-api-openapi.yml
  format: yaml
  label: SimpleVoIP Music on Hold API
  slug: simplevoip-music-on-hold-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-music-on-hold-api-openapi.yml
- filename: simplevoip-sms-api-openapi.yml
  format: yaml
  label: SimpleVoIP SMS API
  slug: simplevoip-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-sms-api-openapi.yml
- filename: simplevoip-time-of-day-api-openapi.yml
  format: yaml
  label: SimpleVoIP Time of Day API
  slug: simplevoip-time-of-day-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-time-of-day-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Simplevoip Authentication
name_suffix: Authentication
oauth_flows: []
overview: SimpleVoIP declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SimpleVoIP
provider_slug: simplevoip
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token authentication required for most endpoints.
  scheme: bearer
  type: http
slug: simplevoip-authentication
source_filename: simplevoip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/simplevoip-openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token authentication required for most endpoints.\n"
source_yaml_url: https://artifacts.apis.io/simplevoip/authentication/simplevoip-authentication.yml
summary_line: 1 scheme
tags:
- VoIP
- Communications
- UCaaS
- AI
- SMB
---
