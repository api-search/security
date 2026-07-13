---
api_key_in:
- header
api_specs:
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Applications API
  slug: edgegap-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap App Versions API
  slug: edgegap-app-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Deployments API
  slug: edgegap-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Sessions API
  slug: edgegap-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Matchmaking API
  slug: edgegap-matchmaking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Relays API
  slug: edgegap-relays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Metrics API
  slug: edgegap-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Fleets API
  slug: edgegap-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Edgegap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edgegap secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Edgegap
provider_slug: edgegap
scheme_count: 1
schemes:
- description: 'API token generated in the Edgegap dashboard (User Settings / Tokens), sent as `Authorization: token <your_token>`.'
  in: header
  name: AuthToken
  parameter: Authorization
  sources:
  - openapi/edgegap-openapi.yml
  type: apiKey
slug: edgegap-authentication
source_filename: edgegap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/edgegap-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AuthToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API token generated in the Edgegap dashboard (User Settings / Tokens), sent\n    as `Authorization: token <your_token>`.'\n  sources:\n  - openapi/edgegap-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/authentication/edgegap-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Game Servers
- Orchestration
- Edge Computing
- Matchmaking
- Hosting
---
