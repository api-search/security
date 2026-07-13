---
api_key_in: []
api_specs:
- filename: rabbitmq-management.yml
  format: yaml
  label: RabbitMQ Management HTTP API
  slug: rabbitmq-management-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-management.yml
- filename: rabbitmq-messaging.yml
  format: yaml
  label: RabbitMQ AMQP Messaging API
  slug: rabbitmq-amqp-messaging-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/asyncapi/rabbitmq-messaging.yml
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
