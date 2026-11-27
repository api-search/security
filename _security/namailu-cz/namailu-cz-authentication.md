---
anonymous_access: false
api_key_in: []
api_specs:
- filename: namailu-cz-acp-api-openapi.yml
  format: yaml
  label: namailu.cz Acp API
  slug: namailu-cz-acp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-acp-api-openapi.yml
- filename: namailu-cz-device-api-openapi.yml
  format: yaml
  label: namailu.cz Device API
  slug: namailu-cz-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-device-api-openapi.yml
- filename: namailu-cz-health-api-openapi.yml
  format: yaml
  label: namailu.cz Health API
  slug: namailu-cz-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-health-api-openapi.yml
- filename: namailu-cz-inboxes-api-openapi.yml
  format: yaml
  label: namailu.cz Inboxes API
  slug: namailu-cz-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-inboxes-api-openapi.yml
- filename: namailu-cz-key-rotation-api-openapi.yml
  format: yaml
  label: namailu.cz Key Rotation API
  slug: namailu-cz-key-rotation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-key-rotation-api-openapi.yml
- filename: namailu-cz-messages-api-openapi.yml
  format: yaml
  label: namailu.cz Messages API
  slug: namailu-cz-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-messages-api-openapi.yml
- filename: namailu-cz-metrics-api-openapi.yml
  format: yaml
  label: namailu.cz Metrics API
  slug: namailu-cz-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-metrics-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: namailu.cz Authentication
name_suffix: Authentication
oauth_flows: []
overview: namailu.cz secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: namailu.cz
provider_slug: namailu-cz
scheme_count: 1
schemes:
- bearerFormat: dmk_live_…
  description: Tenant or inbox API key. Never put it in a query string.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/namailu-cz-openapi.json
  type: http
slug: namailu-cz-authentication
source_filename: namailu-cz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/namailu-cz-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: dmk_live_…\n  description: Tenant or inbox API key. Never put it in a query string.\n  sources:\n  - openapi/namailu-cz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/namailu-cz/authentication/namailu-cz-authentication.yml
summary_line: http · 1 scheme
tags:
- Email Hosting
- AI Agents
- Webmail
- Organisations
---
