---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: live-earnings-com-auth-api-openapi.yml
  format: yaml
  label: Live Earnings Auth API
  slug: live-earnings-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/live-earnings-com/openapi/live-earnings-com-auth-api-openapi.yml
- filename: live-earnings-com-companies-api-openapi.yml
  format: yaml
  label: Live Earnings Companies API
  slug: live-earnings-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/live-earnings-com/openapi/live-earnings-com-companies-api-openapi.yml
- filename: live-earnings-com-events-api-openapi.yml
  format: yaml
  label: Live Earnings Events API
  slug: live-earnings-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/live-earnings-com/openapi/live-earnings-com-events-api-openapi.yml
- filename: live-earnings-com-meta-api-openapi.yml
  format: yaml
  label: Live Earnings Meta API
  slug: live-earnings-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/live-earnings-com/openapi/live-earnings-com-meta-api-openapi.yml
- filename: live-earnings-com-operator-api-openapi.yml
  format: yaml
  label: Live Earnings Operator API
  slug: live-earnings-com-operator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/live-earnings-com/openapi/live-earnings-com-operator-api-openapi.yml
- filename: live-earnings-com-report-api-openapi.yml
  format: yaml
  label: Live Earnings Report API
  slug: live-earnings-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/live-earnings-com/openapi/live-earnings-com-report-api-openapi.yml
- filename: live-earnings-com-sections-api-openapi.yml
  format: yaml
  label: Live Earnings Sections API
  slug: live-earnings-com-sections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/live-earnings-com/openapi/live-earnings-com-sections-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Live Earnings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Live Earnings secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Live Earnings
provider_slug: live-earnings-com
scheme_count: 2
schemes:
- bearerFormat: ek_*
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/live-earnings-com-openapi.yaml
  type: http
- description: DEPRECATED — the subscriber key in the query string (keys in URLs leak into logs). Still accepted. Browsers should mint a session token via POST /api/live/{slug}/session-token and use `?t=` on streams instead.
  in: query
  name: queryToken
  parameter: token
  sources:
  - openapi/live-earnings-com-openapi.yaml
  type: apiKey
slug: live-earnings-com-authentication
source_filename: live-earnings-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/live-earnings-com-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: ek_*\n  sources:\n  - openapi/live-earnings-com-openapi.yaml\n- name: queryToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: DEPRECATED — the subscriber key in the query string (keys in URLs leak into logs).\n    Still accepted. Browsers should mint a session token via POST /api/live/{slug}/session-token\n    and use `?t=` on streams instead.\n  sources:\n  - openapi/live-earnings-com-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/live-earnings-com/authentication/live-earnings-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Earnings Calls
- Live Transcript
- SDK
- Trading Desk
---
