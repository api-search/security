---
api_key_in: []
api_specs:
- filename: gridshare-partner-api-openapi.yml
  format: yaml
  label: Gridshare Partner API
  slug: gridshare-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/gridshare-partner-api-openapi.yml
- filename: gridshare-customer-api-openapi.yml
  format: yaml
  label: Gridshare Customer API
  slug: gridshare-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/gridshare-customer-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Lunar Energy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lunar Energy secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lunar Energy
provider_slug: lunar-energy
scheme_count: 2
schemes:
- description: 'OAuth 2.0 Authorization Code flow against the lunar-customer

    Amazon Cognito user pool.'
  flows:
  - authorizationUrl: https://lunar-customer-prod-us-west-1.auth.us-west-1.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://lunar-customer-prod-us-west-1.auth.us-west-1.amazoncognito.com/oauth2/token
  name: bearerAuth
  sources:
  - openapi/gridshare-customer-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  description: 'OAuth 2.0 client-credentials access token obtained from the

    Gridshare partner Cognito authentication endpoint.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gridshare-partner-api-openapi.yml
  type: http
slug: lunar-energy-authentication
source_filename: lunar-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gridshare-customer-api-openapi.yml, openapi/gridshare-partner-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://lunar-customer-prod-us-west-1.auth.us-west-1.amazoncognito.com/oauth2/authorize\n    tokenUrl: https://lunar-customer-prod-us-west-1.auth.us-west-1.amazoncognito.com/oauth2/token\n    scopes: 4\n  description: |-\n    OAuth 2.0 Authorization Code flow against the lunar-customer\n    Amazon Cognito user pool.\n  sources:\n  - openapi/gridshare-customer-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    OAuth 2.0 client-credentials access token obtained from the\n    Gridshare partner Cognito authentication endpoint.\n  sources:\n  - openapi/gridshare-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/authentication/lunar-energy-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Energy
- Home Battery
- Solar
- Virtual Power Plant
- DERMS
- Distributed Energy Resources
- Grid Services
- Demand Response
- Storage
- Inverter
- Smart Home
- Energy Management
- Tariffs
- Telemetry
- VPP
- Flex Events
---
