---
api_key_in: []
api_specs:
- filename: catchpoint-rest-api-v2-openapi-original.json
  format: json
  label: Catchpoint REST API v2
  slug: catchpoint-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catchpoint/refs/heads/main/openapi/catchpoint-rest-api-v2-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Catchpoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Catchpoint secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Catchpoint
provider_slug: catchpoint
scheme_count: 1
schemes:
- bearerFormat: JWT
  header: Authorization
  in: header
  name: bearer
  scheme: bearer
  sources:
  - openapi/catchpoint-rest-api-v2-openapi-original.json
  type: http
slug: catchpoint-authentication
source_filename: catchpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/catchpoint-rest-api-v2-openapi-original.json\ndocs: https://docs.catchpoint.com/docs/rest-api-v2-guide\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  header: Authorization\n  sources:\n  - openapi/catchpoint-rest-api-v2-openapi-original.json\ndocs_detail:\n  model: api-key-as-bearer-token\n  description: >-\n    Catchpoint's REST API v2 authenticates every request with a REST API key passed\n    as a bearer token in the Authorization header. Keys are created in the Catchpoint\n    Portal under Settings > Integrations > REST API by adding a Consumer and are shown\n    once at creation.\n  key_scope:\n  - client-level (access client data)\n  - division-level (access division data)\n  key_validity: REST API keys are valid for two years from generation; regenerating restarts the two-year window; keys can be revoked.\n\
  \  rotation:\n    supported: true\n    detail: >-\n      Rotational API key support allows account-level key expiration (configurable 30\n      days to 2 years) and up to two active keys per consumer for zero-downtime rotation.\n  reference: https://docs.catchpoint.com/docs/rest-api-v2-guide\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catchpoint/refs/heads/main/authentication/catchpoint-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Devops
- Monitoring
- Observability
- Internet Performance Monitoring
- Synthetic Monitoring
- Real User Monitoring
- Network Monitoring
- BGP Monitoring
- Digital Experience Monitoring
---
