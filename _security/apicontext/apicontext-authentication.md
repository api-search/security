---
api_key_in:
- query
api_specs:
- filename: apicontext-agents-api-openapi.yml
  format: yaml
  label: APIContext Agents API
  slug: apicontext-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-agents-api-openapi.yml
- filename: apicontext-alerts-api-openapi.yml
  format: yaml
  label: APIContext Alerts API
  slug: apicontext-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-alerts-api-openapi.yml
- filename: apicontext-api-calls-api-openapi.yml
  format: yaml
  label: APIContext API Calls API
  slug: apicontext-api-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-api-calls-api-openapi.yml
- filename: apicontext-directory-api-openapi.yml
  format: yaml
  label: APIContext Directory API
  slug: apicontext-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-directory-api-openapi.yml
- filename: apicontext-insights-api-openapi.yml
  format: yaml
  label: APIContext Insights API
  slug: apicontext-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-insights-api-openapi.yml
- filename: apicontext-projects-api-openapi.yml
  format: yaml
  label: APIContext Projects API
  slug: apicontext-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-projects-api-openapi.yml
- filename: apicontext-reports-api-openapi.yml
  format: yaml
  label: APIContext Reports API
  slug: apicontext-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-reports-api-openapi.yml
- filename: apicontext-results-api-openapi.yml
  format: yaml
  label: APIContext Results API
  slug: apicontext-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-results-api-openapi.yml
- filename: apicontext-schedules-api-openapi.yml
  format: yaml
  label: APIContext Schedules API
  slug: apicontext-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-schedules-api-openapi.yml
- filename: apicontext-statistics-api-openapi.yml
  format: yaml
  label: APIContext Statistics API
  slug: apicontext-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-statistics-api-openapi.yml
- filename: apicontext-tokens-api-openapi.yml
  format: yaml
  label: APIContext Tokens API
  slug: apicontext-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-tokens-api-openapi.yml
- filename: apicontext-workflows-api-openapi.yml
  format: yaml
  label: APIContext Workflows API
  slug: apicontext-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apicontext Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIContext secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: APIContext
provider_slug: apicontext
scheme_count: 1
schemes:
- in: query
  name: ApiTokenAuth
  parameter: _token
  sources:
  - openapi/apicontext-platform-openapi.yaml
  type: apiKey
slug: apicontext-authentication
source_filename: apicontext-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apicontext-platform-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiTokenAuth\n  type: apiKey\n  in: query\n  parameter: _token\n  sources:\n  - openapi/apicontext-platform-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/authentication/apicontext-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Directory
- API Monitoring
- Conformance
- Performance
- Platform
- SLO
- Synthetic Testing
- Testing
---
