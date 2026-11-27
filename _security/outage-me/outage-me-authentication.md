---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: outage-me-contribute-api-key-opt-in-api-openapi.yml
  format: yaml
  label: outage.me Contribute — API key, opt-in API
  slug: outage-me-contribute-api-key-opt-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outage-me/openapi/outage-me-contribute-api-key-opt-in-api-openapi.yml
- filename: outage-me-layer-1-open-no-key-api-openapi.yml
  format: yaml
  label: outage.me Layer 1 — open, no key API
  slug: outage-me-layer-1-open-no-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outage-me/openapi/outage-me-layer-1-open-no-key-api-openapi.yml
- filename: outage-me-layer-2-api-key-api-openapi.yml
  format: yaml
  label: outage.me Layer 2 — API key API
  slug: outage-me-layer-2-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outage-me/openapi/outage-me-layer-2-api-key-api-openapi.yml
- filename: outage-me-webhooks-pro-api-key-api-openapi.yml
  format: yaml
  label: outage.me Webhooks — Pro API key API
  slug: outage-me-webhooks-pro-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outage-me/openapi/outage-me-webhooks-pro-api-key-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: outage.me Authentication
name_suffix: Authentication
oauth_flows: []
overview: outage.me secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: outage.me
provider_slug: outage-me
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: x-tarantula-api-key
  sources:
  - openapi/outage-me-openapi.json
  type: apiKey
slug: outage-me-authentication
source_filename: outage-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/outage-me-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-tarantula-api-key\n  sources:\n  - openapi/outage-me-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/outage-me/authentication/outage-me-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Status
- Monitoring
- Real-Time
- Cloud
---
