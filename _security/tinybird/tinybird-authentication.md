---
api_key_in: []
api_specs:
- filename: tinybird-analyze-api-openapi.yml
  format: yaml
  label: Tinybird Analyze API
  slug: tinybird-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-analyze-api-openapi.yml
- filename: tinybird-data-sources-api-openapi.yml
  format: yaml
  label: Tinybird Data Sources API
  slug: tinybird-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-data-sources-api-openapi.yml
- filename: tinybird-environment-variables-api-openapi.yml
  format: yaml
  label: Tinybird Environment Variables API
  slug: tinybird-environment-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-environment-variables-api-openapi.yml
- filename: tinybird-events-api-openapi.yml
  format: yaml
  label: Tinybird Events API
  slug: tinybird-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-events-api-openapi.yml
- filename: tinybird-jobs-api-openapi.yml
  format: yaml
  label: Tinybird Jobs API
  slug: tinybird-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-jobs-api-openapi.yml
- filename: tinybird-organizations-api-openapi.yml
  format: yaml
  label: Tinybird Organizations API
  slug: tinybird-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-organizations-api-openapi.yml
- filename: tinybird-pipes-api-openapi.yml
  format: yaml
  label: Tinybird Pipes API
  slug: tinybird-pipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-pipes-api-openapi.yml
- filename: tinybird-query-api-openapi.yml
  format: yaml
  label: Tinybird Query API
  slug: tinybird-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-query-api-openapi.yml
- filename: tinybird-sink-pipes-api-openapi.yml
  format: yaml
  label: Tinybird Sink Pipes API
  slug: tinybird-sink-pipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-sink-pipes-api-openapi.yml
- filename: tinybird-tokens-api-openapi.yml
  format: yaml
  label: Tinybird Tokens API
  slug: tinybird-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-tokens-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tinybird Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tinybird secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tinybird
provider_slug: tinybird
scheme_count: 1
schemes:
- description: Tinybird authentication token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tinybird-openapi.yml
  type: http
slug: tinybird-authentication
source_filename: tinybird-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tinybird-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Tinybird authentication token\n  sources:\n  - openapi/tinybird-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/authentication/tinybird-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Data
- Real-Time
- SQL
- Streaming
---
