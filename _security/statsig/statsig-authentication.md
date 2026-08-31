---
api_key_in:
- header
api_specs:
- filename: statsig-events-api-openapi.yml
  format: yaml
  label: Statsig Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-events-api-openapi.yml
- filename: statsig-audit-logs-api-openapi.yml
  format: yaml
  label: statsig Audit Logs API
  slug: statsig-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-audit-logs-api-openapi.yml
- filename: statsig-autotunes-api-openapi.yml
  format: yaml
  label: statsig Autotunes API
  slug: statsig-autotunes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-autotunes-api-openapi.yml
- filename: statsig-configuration-api-openapi.yml
  format: yaml
  label: statsig Configuration API
  slug: statsig-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-configuration-api-openapi.yml
- filename: statsig-dynamic-configs-api-openapi.yml
  format: yaml
  label: statsig Dynamic Configs API
  slug: statsig-dynamic-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-dynamic-configs-api-openapi.yml
- filename: statsig-experiments-api-openapi.yml
  format: yaml
  label: statsig Experiments API
  slug: statsig-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-experiments-api-openapi.yml
- filename: statsig-feature-gates-api-openapi.yml
  format: yaml
  label: statsig Feature Gates API
  slug: statsig-feature-gates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-feature-gates-api-openapi.yml
- filename: statsig-gates-api-openapi.yml
  format: yaml
  label: statsig Gates API
  slug: statsig-gates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-gates-api-openapi.yml
- filename: statsig-holdouts-api-openapi.yml
  format: yaml
  label: statsig Holdouts API
  slug: statsig-holdouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-holdouts-api-openapi.yml
- filename: statsig-initialization-api-openapi.yml
  format: yaml
  label: statsig Initialization API
  slug: statsig-initialization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-initialization-api-openapi.yml
- filename: statsig-keys-api-openapi.yml
  format: yaml
  label: statsig Keys API
  slug: statsig-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-keys-api-openapi.yml
- filename: statsig-layers-api-openapi.yml
  format: yaml
  label: statsig Layers API
  slug: statsig-layers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-layers-api-openapi.yml
- filename: statsig-metrics-api-openapi.yml
  format: yaml
  label: statsig Metrics API
  slug: statsig-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-metrics-api-openapi.yml
- filename: statsig-segments-api-openapi.yml
  format: yaml
  label: statsig Segments API
  slug: statsig-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-segments-api-openapi.yml
- filename: statsig-tags-api-openapi.yml
  format: yaml
  label: statsig Tags API
  slug: statsig-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-tags-api-openapi.yml
- filename: statsig-target-apps-api-openapi.yml
  format: yaml
  label: statsig Target Apps API
  slug: statsig-target-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-target-apps-api-openapi.yml
- filename: statsig-users-api-openapi.yml
  format: yaml
  label: statsig Users API
  slug: statsig-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Statsig Authentication
name_suffix: Authentication
oauth_flows: []
overview: statsig secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: statsig
provider_slug: statsig
scheme_count: 2
schemes:
- description: Client-SDK Key that is safe to embed in mobile apps and front-end web applications. Created in Project Settings > API Keys tab.
  in: header
  name: clientSdkKey
  parameter: statsig-api-key
  sources:
  - openapi/statsig-client-sdk-api-openapi.yml
  - openapi/statsig-events-api-openapi.yml
  - openapi/statsig-http-api-openapi.yml
  - openapi/statsig-server-sdk-api-openapi.yml
  type: apiKey
- description: Console API Key created in Project Settings > API Keys tab. Required for all Console API requests.
  in: header
  name: consoleApiKey
  parameter: STATSIG-API-KEY
  sources:
  - openapi/statsig-console-api-openapi.yml
  type: apiKey
slug: statsig-authentication
source_filename: statsig-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/statsig-client-sdk-api-openapi.yml, openapi/statsig-console-api-openapi.yml,\n  openapi/statsig-events-api-openapi.yml, openapi/statsig-http-api-openapi.yml, openapi/statsig-server-sdk-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: clientSdkKey\n  type: apiKey\n  in: header\n  parameter: statsig-api-key\n  description: Client-SDK Key that is safe to embed in mobile apps and front-end web applications.\n    Created in Project Settings > API Keys tab.\n  sources:\n  - openapi/statsig-client-sdk-api-openapi.yml\n  - openapi/statsig-events-api-openapi.yml\n  - openapi/statsig-http-api-openapi.yml\n  - openapi/statsig-server-sdk-api-openapi.yml\n- name: consoleApiKey\n  type: apiKey\n  in: header\n  parameter: STATSIG-API-KEY\n  description: Console API Key created in Project Settings > API Keys tab. Required for all\n    Console API requests.\n  sources:\n  - openapi/statsig-console-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/authentication/statsig-authentication.yml
summary_line: apiKey · 2 schemes
tags: []
---
