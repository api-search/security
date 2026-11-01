---
anonymous_access: false
api_key_in: []
api_specs:
- filename: evcc-auth-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Auth API
  slug: evcc-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-auth-api-openapi.yml
- filename: evcc-battery-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Battery API
  slug: evcc-battery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-battery-api-openapi.yml
- filename: evcc-db-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Db API
  slug: evcc-db-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-db-api-openapi.yml
- filename: evcc-experimental-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Experimental API
  slug: evcc-experimental-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-experimental-api-openapi.yml
- filename: evcc-general-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) General API
  slug: evcc-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-general-api-openapi.yml
- filename: evcc-loadpoints-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Loadpoints API
  slug: evcc-loadpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-loadpoints-api-openapi.yml
- filename: evcc-sessions-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Sessions API
  slug: evcc-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-sessions-api-openapi.yml
- filename: evcc-state-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) State API
  slug: evcc-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-state-api-openapi.yml
- filename: evcc-system-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) System API
  slug: evcc-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-system-api-openapi.yml
- filename: evcc-tariffs-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Tariffs API
  slug: evcc-tariffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-tariffs-api-openapi.yml
- filename: evcc-vehicles-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Vehicles API
  slug: evcc-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-vehicles-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Evcc Authentication
name_suffix: Authentication
oauth_flows: []
overview: evcc (self-hosted) declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: evcc (self-hosted)
provider_slug: evcc
scheme_count: 2
schemes:
- description: Cookie based auth (auth cookie)
  in: cookie
  name: cookieAuth
  official: true
  type: apiKey
- bearerFormat: JWT
  description: Long-lived API key prefixed `evcc_`
  name: bearerAuth
  official: true
  scheme: bearer
  type: http
slug: evcc-authentication
source_filename: evcc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource:\n  - url: https://docs.evcc.io/openapi.yaml\n    note: OpenAPI spec defines authentication schemes\nschemes:\n  - type: apiKey\n    name: cookieAuth\n    in: cookie\n    description: \"Cookie based auth (auth cookie)\"\n    official: true\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    name: bearerAuth\n    description: \"Long-lived API key prefixed `evcc_`\"\n    official: true\n"
source_yaml_url: https://artifacts.apis.io/evcc/authentication/evcc-authentication.yml
summary_line: 2 schemes
tags:
- Company
- EV
- SmartCharging
- OpenSource
- EnergyManagement
- HomeAutomation
---
