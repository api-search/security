---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: HiveMQ REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://docs.hivemq.com/hivemq/latest/rest-api/specification/
- filename: hivemq-asyncapi.yml
  format: yaml
  label: HiveMQ MQTT over WebSocket
  slug: mqtt-websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/hivemq/refs/heads/main/asyncapi/hivemq-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hivemq Authentication
name_suffix: Authentication
oauth_flows: []
overview: HiveMQ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HiveMQ
provider_slug: hivemq
scheme_count: 1
schemes:
- description: 'Authentication is disabled by default. When enabled via the

    HiveMQ Enterprise Security Extension or Enterprise Extension SDK

    REST Service, a bearer token is required.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/hivemq-openapi.yml
  type: http
slug: hivemq-authentication
source_filename: hivemq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hivemq-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Authentication is disabled by default. When enabled via the\n    HiveMQ Enterprise Security Extension or Enterprise Extension SDK\n    REST Service, a bearer token is required.\n  sources:\n  - openapi/hivemq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hivemq/refs/heads/main/authentication/hivemq-authentication.yml
summary_line: http · 1 scheme
tags:
- MQTT
- IoT
- Messaging
- Message Broker
- Pub Sub
- WebSocket
---
