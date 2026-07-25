---
api_key_in: []
api_specs:
- filename: hyperping-healthchecks-api-openapi.yml
  format: yaml
  label: Hyperping Healthchecks API
  slug: hyperping-healthchecks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-healthchecks-api-openapi.yml
- filename: hyperping-incidents-api-openapi.yml
  format: yaml
  label: Hyperping Incidents API
  slug: hyperping-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-incidents-api-openapi.yml
- filename: hyperping-maintenance-api-openapi.yml
  format: yaml
  label: Hyperping Maintenance API
  slug: hyperping-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-maintenance-api-openapi.yml
- filename: hyperping-monitors-api-openapi.yml
  format: yaml
  label: Hyperping Monitors API
  slug: hyperping-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-monitors-api-openapi.yml
- filename: hyperping-outages-api-openapi.yml
  format: yaml
  label: Hyperping Outages API
  slug: hyperping-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-outages-api-openapi.yml
- filename: hyperping-reports-api-openapi.yml
  format: yaml
  label: Hyperping Reports API
  slug: hyperping-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-reports-api-openapi.yml
- filename: hyperping-status-pages-api-openapi.yml
  format: yaml
  label: Hyperping Status Pages API
  slug: hyperping-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-status-pages-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hyperping Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hyperping secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hyperping
provider_slug: hyperping
scheme_count: 1
schemes:
- description: 'Project API key issued from the Developers tab in project settings, sent as `Authorization: Bearer $USER_API_KEY`. Keys can be Read & Write or Read-only. A missing or invalid key returns 401; insufficient permissions return 403.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hyperping-openapi.yml
  type: http
slug: hyperping-authentication
source_filename: hyperping-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hyperping-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Project API key issued from the Developers tab in project settings, sent as\n    `Authorization: Bearer $USER_API_KEY`. Keys can be Read & Write or Read-only. A missing\n    or invalid key returns 401; insufficient permissions return 403.'\n  sources:\n  - openapi/hyperping-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/authentication/hyperping-authentication.yml
summary_line: http · 1 scheme
tags:
- Uptime Monitoring
- Status Pages
- Incident Management
- Observability
- On-Call
---
