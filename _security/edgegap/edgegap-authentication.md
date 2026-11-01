---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: edgegap-applications-api-openapi.yml
  format: yaml
  label: Edgegap Applications API
  slug: edgegap-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgegap/openapi/edgegap-applications-api-openapi.yml
- filename: edgegap-deployments-api-openapi.yml
  format: yaml
  label: Edgegap Deployments API
  slug: edgegap-deployments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgegap/openapi/edgegap-deployments-api-openapi.yml
- filename: edgegap-fleets-api-openapi.yml
  format: yaml
  label: Edgegap Fleets API
  slug: edgegap-fleets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgegap/openapi/edgegap-fleets-api-openapi.yml
- filename: edgegap-metrics-api-openapi.yml
  format: yaml
  label: Edgegap Metrics API
  slug: edgegap-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgegap/openapi/edgegap-metrics-api-openapi.yml
- filename: edgegap-relays-api-openapi.yml
  format: yaml
  label: Edgegap Relays API
  slug: edgegap-relays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgegap/openapi/edgegap-relays-api-openapi.yml
- filename: edgegap-sessions-api-openapi.yml
  format: yaml
  label: Edgegap Sessions API
  slug: edgegap-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgegap/openapi/edgegap-sessions-api-openapi.yml
- filename: edgegap-container-registry-api-openapi.yml
  format: yaml
  label: Edgegap Container Registry API
  slug: edgegap-container-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgegap/openapi/edgegap-container-registry-api-openapi.yml
- filename: edgegap-deployment-tags-api-openapi.yml
  format: yaml
  label: Edgegap Deployment Tags API
  slug: edgegap-deployment-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgegap/openapi/edgegap-deployment-tags-api-openapi.yml
- filename: edgegap-endpoint-storage-api-openapi.yml
  format: yaml
  label: Edgegap Endpoint Storage API
  slug: edgegap-endpoint-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgegap/openapi/edgegap-endpoint-storage-api-openapi.yml
- filename: edgegap-ip-lookup-api-openapi.yml
  format: yaml
  label: Edgegap IP Lookup API
  slug: edgegap-ip-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgegap/openapi/edgegap-ip-lookup-api-openapi.yml
- filename: edgegap-locations-api-openapi.yml
  format: yaml
  label: Edgegap Locations API
  slug: edgegap-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgegap/openapi/edgegap-locations-api-openapi.yml
- filename: edgegap-report-deployment-api-openapi.yml
  format: yaml
  label: Edgegap Report Deployment API
  slug: edgegap-report-deployment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgegap/openapi/edgegap-report-deployment-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/edgegap/authentication/edgegap-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Game Servers
- Edge Computing
- Matchmaking
- Hosting
- Container Orchestration
---
