---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: hotelumo-com-availability-api-openapi.yml
  format: yaml
  label: Hotelumo Availability API
  slug: hotelumo-com-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotelumo-com/openapi/hotelumo-com-availability-api-openapi.yml
- filename: hotelumo-com-daily-rates-api-openapi.yml
  format: yaml
  label: Hotelumo Daily rates API
  slug: hotelumo-com-daily-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotelumo-com/openapi/hotelumo-com-daily-rates-api-openapi.yml
- filename: hotelumo-com-guests-api-openapi.yml
  format: yaml
  label: Hotelumo Guests API
  slug: hotelumo-com-guests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotelumo-com/openapi/hotelumo-com-guests-api-openapi.yml
- filename: hotelumo-com-rate-plans-api-openapi.yml
  format: yaml
  label: Hotelumo Rate plans API
  slug: hotelumo-com-rate-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotelumo-com/openapi/hotelumo-com-rate-plans-api-openapi.yml
- filename: hotelumo-com-reservations-api-openapi.yml
  format: yaml
  label: Hotelumo Reservations API
  slug: hotelumo-com-reservations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotelumo-com/openapi/hotelumo-com-reservations-api-openapi.yml
- filename: hotelumo-com-room-types-api-openapi.yml
  format: yaml
  label: Hotelumo Room types API
  slug: hotelumo-com-room-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotelumo-com/openapi/hotelumo-com-room-types-api-openapi.yml
- filename: hotelumo-com-rooms-api-openapi.yml
  format: yaml
  label: Hotelumo Rooms API
  slug: hotelumo-com-rooms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotelumo-com/openapi/hotelumo-com-rooms-api-openapi.yml
- filename: hotelumo-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Hotelumo Webhook subscriptions API
  slug: hotelumo-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotelumo-com/openapi/hotelumo-com-webhook-subscriptions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Hotelumo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hotelumo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hotelumo
provider_slug: hotelumo-com
scheme_count: 2
schemes:
- description: 'HTTP Basic auth carrying only the API key secret: `Authorization: Basic base64(<key secret>)`.'
  name: apiKey
  scheme: basic
  sources:
  - openapi/hotelumo-com-openapi.json
  type: http
- description: 'Operator session token issued by the Hotelumo dashboard: `Authorization: Token <access token>`.'
  in: header
  name: accessToken
  parameter: Authorization
  sources:
  - openapi/hotelumo-com-openapi.json
  type: apiKey
slug: hotelumo-com-authentication
source_filename: hotelumo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hotelumo-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: http\n  scheme: basic\n  description: 'HTTP Basic auth carrying only the API key secret: `Authorization: Basic base64(<key\n    secret>)`.'\n  sources:\n  - openapi/hotelumo-com-openapi.json\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Operator session token issued by the Hotelumo dashboard: `Authorization: Token\n    <access token>`.'\n  sources:\n  - openapi/hotelumo-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hotelumo-com/authentication/hotelumo-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Hotel Management
- Hospitality
- Software-as-a-Service
- Reservations
- Guest Services
- Company
---
