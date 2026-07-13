---
api_key_in: []
api_specs:
- filename: snowplow-console-api-openapi.yml
  format: yaml
  label: Snowplow Console API
  slug: snowplow-console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowplow/refs/heads/main/openapi/snowplow-console-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Snowplow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snowplow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Snowplow
provider_slug: snowplow
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token obtained from the Credentials API (/credentials/v3/token)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/snowplow-console-api-openapi.yml
  type: http
slug: snowplow-authentication
source_filename: snowplow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snowplow-console-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained from the Credentials API (/credentials/v3/token)\n  sources:\n  - openapi/snowplow-console-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snowplow/refs/heads/main/authentication/snowplow-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics Platform
- Behavioral Data
- Data Collection
- Data Engineering
- Data Pipeline
- Event Tracking
- Open Source
---
