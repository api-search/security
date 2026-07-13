---
api_key_in:
- header
api_specs:
- filename: statsig-http-api-openapi.yml
  format: yaml
  label: Statsig HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-http-api-openapi.yml
- filename: statsig-console-api-openapi.yml
  format: yaml
  label: Statsig Console API
  slug: console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-console-api-openapi.yml
- filename: statsig-client-sdk-api-openapi.yml
  format: yaml
  label: Statsig Client SDK API
  slug: client-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-client-sdk-api-openapi.yml
- filename: statsig-server-sdk-api-openapi.yml
  format: yaml
  label: Statsig Server SDK API
  slug: server-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-server-sdk-api-openapi.yml
- filename: statsig-events-api-openapi.yml
  format: yaml
  label: Statsig Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-events-api-openapi.yml
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
