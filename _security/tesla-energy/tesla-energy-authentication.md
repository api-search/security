---
api_key_in: []
api_specs:
- filename: tesla-energy-backup-api-openapi.yml
  format: yaml
  label: Tesla Energy Backup API
  slug: tesla-energy-backup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-backup-api-openapi.yml
- filename: tesla-energy-history-api-openapi.yml
  format: yaml
  label: Tesla Energy History API
  slug: tesla-energy-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-history-api-openapi.yml
- filename: tesla-energy-live-status-api-openapi.yml
  format: yaml
  label: Tesla Energy Live Status API
  slug: tesla-energy-live-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-live-status-api-openapi.yml
- filename: tesla-energy-off-grid-charging-api-openapi.yml
  format: yaml
  label: Tesla Energy Off Grid Charging API
  slug: tesla-energy-off-grid-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-off-grid-charging-api-openapi.yml
- filename: tesla-energy-operation-api-openapi.yml
  format: yaml
  label: Tesla Energy Operation API
  slug: tesla-energy-operation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-operation-api-openapi.yml
- filename: tesla-energy-products-api-openapi.yml
  format: yaml
  label: Tesla Energy Products API
  slug: tesla-energy-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-products-api-openapi.yml
- filename: tesla-energy-programs-api-openapi.yml
  format: yaml
  label: Tesla Energy Programs API
  slug: tesla-energy-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-programs-api-openapi.yml
- filename: tesla-energy-site-info-api-openapi.yml
  format: yaml
  label: Tesla Energy Site Info API
  slug: tesla-energy-site-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-site-info-api-openapi.yml
- filename: tesla-energy-storm-mode-api-openapi.yml
  format: yaml
  label: Tesla Energy Storm Mode API
  slug: tesla-energy-storm-mode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-storm-mode-api-openapi.yml
- filename: tesla-energy-time-of-use-api-openapi.yml
  format: yaml
  label: Tesla Energy Time Of Use API
  slug: tesla-energy-time-of-use-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-time-of-use-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tesla Energy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tesla Energy secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tesla Energy
provider_slug: tesla-energy
scheme_count: 1
schemes:
- description: Tesla Fleet API OAuth 2.0 with PKCE. Scopes energy_device_data (read) and energy_cmds (write) required for the energy_sites endpoints.
  flows:
  - authorizationUrl: https://auth.tesla.com/oauth2/v3/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://auth.tesla.com/oauth2/v3/token
  name: BearerAuth
  sources:
  - openapi/tesla-energy-fleet-api-openapi.yml
  type: oauth2
slug: tesla-energy-authentication
source_filename: tesla-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tesla-energy-fleet-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.tesla.com/oauth2/v3/authorize\n    tokenUrl: https://auth.tesla.com/oauth2/v3/token\n    scopes: 3\n  description: Tesla Fleet API OAuth 2.0 with PKCE. Scopes energy_device_data (read) and energy_cmds\n    (write) required for the energy_sites endpoints.\n  sources:\n  - openapi/tesla-energy-fleet-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/authentication/tesla-energy-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Energy
- Clean Energy
- Solar
- Battery Storage
- Powerwall
- Megapack
- Solar Roof
- Virtual Power Plant
- IoT
- Grid Services
- Home Energy
- Utility Scale
---
