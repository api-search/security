---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: indianumerology-com-openapi.json
  format: json
  label: Numerology Engine API
  slug: numerology-engine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indianumerology-com/openapi/indianumerology-com-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: India Numerology Authentication
name_suffix: Authentication
oauth_flows: []
overview: India Numerology secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: India Numerology
provider_slug: indianumerology-com
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/indianumerology-com-openapi.json
  type: apiKey
slug: indianumerology-com-authentication
source_filename: indianumerology-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/indianumerology-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/indianumerology-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/indianumerology-com/authentication/indianumerology-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Numerology
- Calculator
- Astrology
- India
---
