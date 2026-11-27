---
anonymous_access: false
api_key_in: []
api_specs:
- filename: daycal-io-owner-api-openapi.yml
  format: yaml
  label: Daycal Owner API
  slug: daycal-io-owner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daycal-io/openapi/daycal-io-owner-api-openapi.yml
- filename: daycal-io-public-api-openapi.yml
  format: yaml
  label: Daycal Public API
  slug: daycal-io-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daycal-io/openapi/daycal-io-public-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Daycal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Daycal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Daycal
provider_slug: daycal-io
scheme_count: 1
schemes:
- description: 'OAuth access token or Daycal API token (daycal_...). Its owner scopes decide which tools and routes it reaches: read, write (includes read), billing, secrets; GET /api/me/tools lists the tools it may call.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/daycal-io-openapi.json
  type: http
slug: daycal-io-authentication
source_filename: daycal-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/daycal-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'OAuth access token or Daycal API token (daycal_...). Its owner scopes decide\n    which tools and routes it reaches: read, write (includes read), billing, secrets; GET /api/me/tools\n    lists the tools it may call.'\n  sources:\n  - openapi/daycal-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/daycal-io/authentication/daycal-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Scheduling
- Calendar
- AI Assistant
- Productivity
- Automation
- Company
---
