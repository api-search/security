---
api_key_in:
- header
api_specs:
- filename: schlage-home-openapi.yml
  format: yaml
  label: Schlage Home API
  slug: schlage-home-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allegion/refs/heads/main/openapi/schlage-home-openapi.yml
- filename: engage-credentialing-openapi.yml
  format: yaml
  label: ENGAGE Cloud Credentialing API
  slug: engage-credentialing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allegion/refs/heads/main/openapi/engage-credentialing-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Allegion Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Allegion secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Allegion
provider_slug: allegion
scheme_count: 3
schemes:
- description: Azure API Management subscription key issued via the Allegion Developer Portal.
  in: header
  name: SubscriptionKey
  parameter: alle-subscription-key
  sources:
  - openapi/engage-credentialing-openapi.yml
  type: apiKey
- description: Basic Auth token generated from ENGAGE credentials.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/engage-credentialing-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://account.schlage.com/OAuth2/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://account.schlage.com/OAuth2/token
  name: OAuth2
  sources:
  - openapi/schlage-home-openapi.yml
  type: oauth2
slug: allegion-authentication
source_filename: allegion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/engage-credentialing-openapi.yml, openapi/schlage-home-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: SubscriptionKey\n  type: apiKey\n  in: header\n  parameter: alle-subscription-key\n  description: Azure API Management subscription key issued via the Allegion Developer Portal.\n  sources:\n  - openapi/engage-credentialing-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Basic Auth token generated from ENGAGE credentials.\n  sources:\n  - openapi/engage-credentialing-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.schlage.com/OAuth2/authorize\n    tokenUrl: https://account.schlage.com/OAuth2/token\n    scopes: 5\n  sources:\n  - openapi/schlage-home-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allegion/refs/heads/main/authentication/allegion-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Access Control
- Smart Lock
- Smart Home
- Mobile Credentials
- Bluetooth
- BLE
- IoT
- Security
- Webhooks
- OAuth
- Schlage
- Von Duprin
- ENGAGE
---
