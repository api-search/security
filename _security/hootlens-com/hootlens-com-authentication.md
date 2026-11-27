---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hootlens-com-account-api-openapi.yml
  format: yaml
  label: Hoot Lens Account API
  slug: hootlens-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-account-api-openapi.yml
- filename: hootlens-com-analysis-api-openapi.yml
  format: yaml
  label: Hoot Lens Analysis API
  slug: hootlens-com-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-analysis-api-openapi.yml
- filename: hootlens-com-changes-api-openapi.yml
  format: yaml
  label: Hoot Lens Changes API
  slug: hootlens-com-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-changes-api-openapi.yml
- filename: hootlens-com-conversions-api-openapi.yml
  format: yaml
  label: Hoot Lens Conversions API
  slug: hootlens-com-conversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-conversions-api-openapi.yml
- filename: hootlens-com-element-names-api-openapi.yml
  format: yaml
  label: Hoot Lens Element names API
  slug: hootlens-com-element-names-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-element-names-api-openapi.yml
- filename: hootlens-com-errors-api-openapi.yml
  format: yaml
  label: Hoot Lens Errors API
  slug: hootlens-com-errors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-errors-api-openapi.yml
- filename: hootlens-com-funnels-api-openapi.yml
  format: yaml
  label: Hoot Lens Funnels API
  slug: hootlens-com-funnels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-funnels-api-openapi.yml
- filename: hootlens-com-goals-api-openapi.yml
  format: yaml
  label: Hoot Lens Goals API
  slug: hootlens-com-goals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-goals-api-openapi.yml
- filename: hootlens-com-heatmaps-api-openapi.yml
  format: yaml
  label: Hoot Lens Heatmaps API
  slug: hootlens-com-heatmaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-heatmaps-api-openapi.yml
- filename: hootlens-com-improvements-api-openapi.yml
  format: yaml
  label: Hoot Lens Improvements API
  slug: hootlens-com-improvements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-improvements-api-openapi.yml
- filename: hootlens-com-install-api-openapi.yml
  format: yaml
  label: Hoot Lens Install API
  slug: hootlens-com-install-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-install-api-openapi.yml
- filename: hootlens-com-recordings-api-openapi.yml
  format: yaml
  label: Hoot Lens Recordings API
  slug: hootlens-com-recordings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-recordings-api-openapi.yml
- filename: hootlens-com-service-api-openapi.yml
  format: yaml
  label: Hoot Lens Service API
  slug: hootlens-com-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-service-api-openapi.yml
- filename: hootlens-com-settings-changes-api-openapi.yml
  format: yaml
  label: Hoot Lens Settings changes API
  slug: hootlens-com-settings-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-settings-changes-api-openapi.yml
- filename: hootlens-com-sites-api-openapi.yml
  format: yaml
  label: Hoot Lens Sites API
  slug: hootlens-com-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-sites-api-openapi.yml
- filename: hootlens-com-visits-api-openapi.yml
  format: yaml
  label: Hoot Lens Visits API
  slug: hootlens-com-visits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-visits-api-openapi.yml
- filename: hootlens-com-webhooks-api-openapi.yml
  format: yaml
  label: Hoot Lens Webhooks API
  slug: hootlens-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hootlens-com/openapi/hootlens-com-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hoot Lens Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hoot Lens secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hoot Lens
provider_slug: hootlens-com
scheme_count: 1
schemes:
- description: A Firebase ID token, or a personal access token (hl_pat_...) with the scopes read, replay, annotate, configure, conversions:write. OAuth access tokens (hl_oat_...) are for the hosted MCP resource only.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hootlens-com-openapi.json
  type: http
slug: hootlens-com-authentication
source_filename: hootlens-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hootlens-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: A Firebase ID token, or a personal access token (hl_pat_...) with the scopes\n    read, replay, annotate, configure, conversions:write. OAuth access tokens (hl_oat_...) are\n    for the hosted MCP resource only.\n  sources:\n  - openapi/hootlens-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hootlens-com/authentication/hootlens-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Session Replay
- Heatmaps
- User Experience
- Software-as-a-Service
- Parallel Platforms
---
