---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: wapiworld-com-instances-api-openapi.yml
  format: yaml
  label: wapiworld-com Instances API
  slug: wapiworld-com-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wapiworld-com/openapi/wapiworld-com-instances-api-openapi.yml
- filename: wapiworld-com-messages-api-openapi.yml
  format: yaml
  label: wapiworld-com Messages API
  slug: wapiworld-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wapiworld-com/openapi/wapiworld-com-messages-api-openapi.yml
- filename: wapiworld-com-projects-api-openapi.yml
  format: yaml
  label: wapiworld-com Projects API
  slug: wapiworld-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wapiworld-com/openapi/wapiworld-com-projects-api-openapi.yml
- filename: wapiworld-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: wapiworld-com Webhook subscriptions API
  slug: wapiworld-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wapiworld-com/openapi/wapiworld-com-webhook-subscriptions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Wapiworld Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: wapiworld-com secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: wapiworld-com
provider_slug: wapiworld-com
scheme_count: 2
schemes:
- description: 'HTTP Basic auth carrying only the API key secret: `Authorization: Basic base64(<key secret>)`.'
  name: apiKey
  scheme: basic
  sources:
  - openapi/wapiworld-com-openapi.json
  type: http
- description: 'Operator session token issued by the Wapiworld dashboard: `Authorization: Token <access token>`.'
  in: header
  name: accessToken
  parameter: Authorization
  sources:
  - openapi/wapiworld-com-openapi.json
  type: apiKey
slug: wapiworld-com-authentication
source_filename: wapiworld-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/wapiworld-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: http\n  scheme: basic\n  description: 'HTTP Basic auth carrying only the API key secret: `Authorization: Basic base64(<key\n    secret>)`.'\n  sources:\n  - openapi/wapiworld-com-openapi.json\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Operator session token issued by the Wapiworld dashboard: `Authorization: Token\n    <access token>`.'\n  sources:\n  - openapi/wapiworld-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/wapiworld-com/authentication/wapiworld-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Messaging
- WhatsApp
- Developer Platform
- Communications
---
