---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Confluent The Data Streaming Platform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Confluent | the Data Streaming Platform secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Confluent | the Data Streaming Platform
provider_slug: confluent-the-data-streaming-platform
scheme_count: 2
schemes:
- description: Cloud API Key (key) and Secret (password)
  name: basicAuth
  scheme: basic
  sources:
  - openapi/confluent-the-data-streaming-platform-openapi.yml
  type: http
- bearerFormat: JWT
  description: Confluent STS or external OAuth access token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/confluent-the-data-streaming-platform-openapi.yml
  type: http
slug: confluent-the-data-streaming-platform-authentication
source_filename: confluent-the-data-streaming-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/confluent-the-data-streaming-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Cloud API Key (key) and Secret (password)\n  sources:\n  - openapi/confluent-the-data-streaming-platform-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Confluent STS or external OAuth access token\n  sources:\n  - openapi/confluent-the-data-streaming-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/authentication/confluent-the-data-streaming-platform-authentication.yml
summary_line: http · 2 schemes
tags:
- Apache Flink
- Apache Kafka
- Confluent Cloud
- Connectors
- Data Streaming
- Event Streaming
- Kafka Connect
- ksqlDB
- Real-Time Data
- REST
- Schema Registry
- Stream Processing
---
