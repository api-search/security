---
api_key_in:
- header
api_specs:
- filename: eaton-authorization-api-openapi.yml
  format: yaml
  label: Eaton Authorization API
  slug: eaton-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-authorization-api-openapi.yml
- filename: eaton-device-commands-api-openapi.yml
  format: yaml
  label: Eaton Device Commands API
  slug: eaton-device-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-device-commands-api-openapi.yml
- filename: eaton-devices-api-openapi.yml
  format: yaml
  label: Eaton Devices API
  slug: eaton-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-devices-api-openapi.yml
- filename: eaton-energy-data-api-openapi.yml
  format: yaml
  label: Eaton Energy Data API
  slug: eaton-energy-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-energy-data-api-openapi.yml
- filename: eaton-ev-only-api-openapi.yml
  format: yaml
  label: Eaton EV Only API
  slug: eaton-ev-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-ev-only-api-openapi.yml
- filename: eaton-events-api-openapi.yml
  format: yaml
  label: Eaton Events API
  slug: eaton-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-events-api-openapi.yml
- filename: eaton-locations-api-openapi.yml
  format: yaml
  label: Eaton Locations API
  slug: eaton-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-locations-api-openapi.yml
- filename: eaton-organizations-api-openapi.yml
  format: yaml
  label: Eaton Organizations API
  slug: eaton-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-organizations-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Eaton Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Eaton secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Eaton
provider_slug: eaton
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.em.eaton.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/smart-breaker-openapi.yml
  type: oauth2
- in: header
  name: SubscriptionKey
  parameter: Em-Api-Subscription-Key
  sources:
  - openapi/smart-breaker-openapi.yml
  type: apiKey
slug: eaton-authentication
source_filename: eaton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smart-breaker-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.em.eaton.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/smart-breaker-openapi.yml\n- name: SubscriptionKey\n  type: apiKey\n  in: header\n  parameter: Em-Api-Subscription-Key\n  sources:\n  - openapi/smart-breaker-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/authentication/eaton-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Power Management
- Electrical
- Smart Breaker
- EV Charging
- Demand Response
- Data Center
- DCIM
- PDU
- UPS
- Utility
- Industrial
- Building
- Mobility
- AI Factory
- Energy
- IoT
- Sustainability
---
