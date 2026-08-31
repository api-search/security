---
api_key_in:
- header
api_specs:
- filename: n8n-audit-api-openapi.yml
  format: yaml
  label: N8n Audit API
  slug: n8n-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-audit-api-openapi.yml
- filename: n8n-communitypackage-api-openapi.yml
  format: yaml
  label: N8n CommunityPackage API
  slug: n8n-communitypackage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-communitypackage-api-openapi.yml
- filename: n8n-credential-api-openapi.yml
  format: yaml
  label: N8n Credential API
  slug: n8n-credential-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-credential-api-openapi.yml
- filename: n8n-datatable-api-openapi.yml
  format: yaml
  label: N8n DataTable API
  slug: n8n-datatable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-datatable-api-openapi.yml
- filename: n8n-discover-api-openapi.yml
  format: yaml
  label: N8n Discover API
  slug: n8n-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-discover-api-openapi.yml
- filename: n8n-execution-api-openapi.yml
  format: yaml
  label: N8n Execution API
  slug: n8n-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-execution-api-openapi.yml
- filename: n8n-folders-api-openapi.yml
  format: yaml
  label: N8n Folders API
  slug: n8n-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-folders-api-openapi.yml
- filename: n8n-insights-api-openapi.yml
  format: yaml
  label: N8n Insights API
  slug: n8n-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-insights-api-openapi.yml
- filename: n8n-projects-api-openapi.yml
  format: yaml
  label: N8n Projects API
  slug: n8n-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-projects-api-openapi.yml
- filename: n8n-sourcecontrol-api-openapi.yml
  format: yaml
  label: N8n SourceControl API
  slug: n8n-sourcecontrol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-sourcecontrol-api-openapi.yml
- filename: n8n-tags-api-openapi.yml
  format: yaml
  label: N8n Tags API
  slug: n8n-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-tags-api-openapi.yml
- filename: n8n-user-api-openapi.yml
  format: yaml
  label: N8n User API
  slug: n8n-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-user-api-openapi.yml
- filename: n8n-variables-api-openapi.yml
  format: yaml
  label: N8n Variables API
  slug: n8n-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-variables-api-openapi.yml
- filename: n8n-workflow-api-openapi.yml
  format: yaml
  label: N8n Workflow API
  slug: n8n-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-workflow-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: N8N Authentication
name_suffix: Authentication
oauth_flows: []
overview: n8n secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: n8n
provider_slug: n8n
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-N8N-API-KEY
  sources:
  - openapi/n8n-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/n8n-openapi.yml
  type: http
slug: n8n-authentication
source_filename: n8n-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/n8n-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-N8N-API-KEY\n  sources:\n  - openapi/n8n-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/n8n-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/authentication/n8n-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Agents
- Artificial Intelligence
- Integration
---
