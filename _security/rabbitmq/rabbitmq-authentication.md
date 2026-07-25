---
api_key_in: []
api_specs:
- filename: rabbitmq-messaging.yml
  format: yaml
  label: RabbitMQ AMQP Messaging API
  slug: rabbitmq-amqp-messaging-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/asyncapi/rabbitmq-messaging.yml
- filename: rabbitmq-bindings-api-openapi.yml
  format: yaml
  label: RabbitMQ Bindings API
  slug: rabbitmq-bindings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-bindings-api-openapi.yml
- filename: rabbitmq-channels-api-openapi.yml
  format: yaml
  label: RabbitMQ Channels API
  slug: rabbitmq-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-channels-api-openapi.yml
- filename: rabbitmq-connections-api-openapi.yml
  format: yaml
  label: RabbitMQ Connections API
  slug: rabbitmq-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-connections-api-openapi.yml
- filename: rabbitmq-definitions-api-openapi.yml
  format: yaml
  label: RabbitMQ Definitions API
  slug: rabbitmq-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-definitions-api-openapi.yml
- filename: rabbitmq-exchanges-api-openapi.yml
  format: yaml
  label: RabbitMQ Exchanges API
  slug: rabbitmq-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-exchanges-api-openapi.yml
- filename: rabbitmq-health-api-openapi.yml
  format: yaml
  label: RabbitMQ Health API
  slug: rabbitmq-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-health-api-openapi.yml
- filename: rabbitmq-nodes-api-openapi.yml
  format: yaml
  label: RabbitMQ Nodes API
  slug: rabbitmq-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-nodes-api-openapi.yml
- filename: rabbitmq-overview-api-openapi.yml
  format: yaml
  label: RabbitMQ Overview API
  slug: rabbitmq-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-overview-api-openapi.yml
- filename: rabbitmq-permissions-api-openapi.yml
  format: yaml
  label: RabbitMQ Permissions API
  slug: rabbitmq-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-permissions-api-openapi.yml
- filename: rabbitmq-policies-api-openapi.yml
  format: yaml
  label: RabbitMQ Policies API
  slug: rabbitmq-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-policies-api-openapi.yml
- filename: rabbitmq-queues-api-openapi.yml
  format: yaml
  label: RabbitMQ Queues API
  slug: rabbitmq-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-queues-api-openapi.yml
- filename: rabbitmq-users-api-openapi.yml
  format: yaml
  label: RabbitMQ Users API
  slug: rabbitmq-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-users-api-openapi.yml
- filename: rabbitmq-virtual-hosts-api-openapi.yml
  format: yaml
  label: RabbitMQ Virtual Hosts API
  slug: rabbitmq-virtual-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-virtual-hosts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rabbitmq Authentication
name_suffix: Authentication
oauth_flows: []
overview: RabbitMQ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RabbitMQ
provider_slug: rabbitmq
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/rabbitmq-management.yml
  type: http
slug: rabbitmq-authentication
source_filename: rabbitmq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rabbitmq-management.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/rabbitmq-management.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/authentication/rabbitmq-authentication.yml
summary_line: http · 1 scheme
tags:
- AMQP
- Distributed Systems
- Event Streaming
- Message Broker
- Messaging
- Queue
---
