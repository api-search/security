---
api_key_in: []
api_specs:
- filename: enode-batteries-api-openapi.yml
  format: yaml
  label: Enode Batteries API
  slug: enode-batteries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-batteries-api-openapi.yml
- filename: enode-chargers-api-openapi.yml
  format: yaml
  label: Enode Chargers API
  slug: enode-chargers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-chargers-api-openapi.yml
- filename: enode-hvac-api-openapi.yml
  format: yaml
  label: Enode HVAC API
  slug: enode-hvac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-hvac-api-openapi.yml
- filename: enode-inverters-api-openapi.yml
  format: yaml
  label: Enode Inverters API
  slug: enode-inverters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-inverters-api-openapi.yml
- filename: enode-meters-api-openapi.yml
  format: yaml
  label: Enode Meters API
  slug: enode-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-meters-api-openapi.yml
- filename: enode-smart-charging-api-openapi.yml
  format: yaml
  label: Enode Smart Charging API
  slug: enode-smart-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-smart-charging-api-openapi.yml
- filename: enode-users-api-openapi.yml
  format: yaml
  label: Enode Users API
  slug: enode-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-users-api-openapi.yml
- filename: enode-vehicles-api-openapi.yml
  format: yaml
  label: Enode Vehicles API
  slug: enode-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-vehicles-api-openapi.yml
- filename: enode-webhooks-api-openapi.yml
  format: yaml
  label: Enode Webhooks API
  slug: enode-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/authentication/enode-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Electric Vehicles
- EV Charging
- Smart Charging
- Energy Transition
---
