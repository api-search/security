---
anonymous_access: false
api_key_in: []
api_specs:
- filename: enode-batteries-api-openapi.yml
  format: yaml
  label: Enode Batteries API
  slug: enode-batteries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-batteries-api-openapi.yml
- filename: enode-chargers-api-openapi.yml
  format: yaml
  label: Enode Chargers API
  slug: enode-chargers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-chargers-api-openapi.yml
- filename: enode-hvac-api-openapi.yml
  format: yaml
  label: Enode HVAC API
  slug: enode-hvac-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-hvac-api-openapi.yml
- filename: enode-meters-api-openapi.yml
  format: yaml
  label: Enode Meters API
  slug: enode-meters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-meters-api-openapi.yml
- filename: enode-vehicles-api-openapi.yml
  format: yaml
  label: Enode Vehicles API
  slug: enode-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-vehicles-api-openapi.yml
- filename: enode-webhooks-api-openapi.yml
  format: yaml
  label: Enode Webhooks API
  slug: enode-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-webhooks-api-openapi.yml
- filename: enode-beta-api-openapi.yml
  format: yaml
  label: Enode Beta API
  slug: enode-beta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-beta-api-openapi.yml
- filename: enode-early-adopter-api-openapi.yml
  format: yaml
  label: Enode Early Adopter API
  slug: enode-early-adopter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-early-adopter-api-openapi.yml
- filename: enode-interventions-api-openapi.yml
  format: yaml
  label: Enode Interventions API
  slug: enode-interventions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-interventions-api-openapi.yml
- filename: enode-locations-api-openapi.yml
  format: yaml
  label: Enode Locations API
  slug: enode-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-locations-api-openapi.yml
- filename: enode-schedules-api-openapi.yml
  format: yaml
  label: Enode Schedules API
  slug: enode-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-schedules-api-openapi.yml
- filename: enode-service-health-api-openapi.yml
  format: yaml
  label: Enode Service Health API
  slug: enode-service-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-service-health-api-openapi.yml
- filename: enode-solar-inverters-api-openapi.yml
  format: yaml
  label: Enode Solar inverters API
  slug: enode-solar-inverters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-solar-inverters-api-openapi.yml
- filename: enode-statistics-api-openapi.yml
  format: yaml
  label: Enode Statistics API
  slug: enode-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-statistics-api-openapi.yml
- filename: enode-tariffs-api-openapi.yml
  format: yaml
  label: Enode Tariffs API
  slug: enode-tariffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-tariffs-api-openapi.yml
- filename: enode-user-management-api-openapi.yml
  format: yaml
  label: Enode User Management API
  slug: enode-user-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-user-management-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Enode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enode secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Enode
provider_slug: enode
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained via the client_credentials grant from the Enode OAuth token endpoint (https://oauth.production.enode.io/oauth2/token for production, https://oauth.sandbox.enode.io/oauth2/token for sandbox), presented as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/enode-openapi.yml
  type: http
slug: enode-authentication
source_filename: enode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/enode-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained via the client_credentials grant from the Enode\n    OAuth token endpoint (https://oauth.production.enode.io/oauth2/token for production, https://oauth.sandbox.enode.io/oauth2/token\n    for sandbox), presented as a Bearer token.\n  sources:\n  - openapi/enode-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/enode/authentication/enode-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Electric Vehicles
- EV Charging
- Smart Charging
- Energy Transition
- Mobility
---
