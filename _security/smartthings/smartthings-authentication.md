---
api_key_in: []
api_specs:
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Devices API
  slug: smartthings-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Device Commands & Status API
  slug: smartthings-device-commands-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Locations API
  slug: smartthings-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Rooms API
  slug: smartthings-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Scenes API
  slug: smartthings-scenes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Rules API
  slug: smartthings-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Capabilities API
  slug: smartthings-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Subscriptions API
  slug: smartthings-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Schedules API
  slug: smartthings-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Apps API
  slug: smartthings-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Installed Apps API
  slug: smartthings-installed-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Presentations API
  slug: smartthings-presentations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings History API
  slug: smartthings-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Virtual Devices API
  slug: smartthings-virtual-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Smartthings Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Samsung SmartThings secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Samsung SmartThings
provider_slug: smartthings
scheme_count: 2
schemes:
- description: 'A Personal Access Token (PAT) from https://account.smartthings.com/tokens or an OAuth 2.0 access token, passed as `Authorization: Bearer {token}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/smartthings-openapi.yml
  type: http
- description: OAuth 2.0 authorization code flow for production integrations.
  flows:
  - authorizationUrl: https://api.smartthings.com/oauth/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://api.smartthings.com/oauth/token
  name: oauth2
  sources:
  - openapi/smartthings-openapi.yml
  type: oauth2
slug: smartthings-authentication
source_filename: smartthings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smartthings-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'A Personal Access Token (PAT) from https://account.smartthings.com/tokens or\n    an OAuth 2.0 access token, passed as `Authorization: Bearer {token}`.'\n  sources:\n  - openapi/smartthings-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.smartthings.com/oauth/authorize\n    tokenUrl: https://api.smartthings.com/oauth/token\n    scopes: 8\n  description: OAuth 2.0 authorization code flow for production integrations.\n  sources:\n  - openapi/smartthings-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/authentication/smartthings-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Smart Home
- IoT
- Home Automation
- Devices
- Samsung
---
