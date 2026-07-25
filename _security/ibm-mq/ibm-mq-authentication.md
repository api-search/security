---
api_key_in:
- cookie
api_specs:
- filename: ibm-mq-messaging-asyncapi.yml
  format: yaml
  label: IBM MQ JMS API
  slug: ibm-mq-jms-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/asyncapi/ibm-mq-messaging-asyncapi.yml
- filename: ibm-mq-channels-api-openapi.yml
  format: yaml
  label: IBM MQ Channels API
  slug: ibm-mq-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-channels-api-openapi.yml
- filename: ibm-mq-installations-api-openapi.yml
  format: yaml
  label: IBM MQ Installations API
  slug: ibm-mq-installations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-installations-api-openapi.yml
- filename: ibm-mq-login-api-openapi.yml
  format: yaml
  label: IBM MQ Login API
  slug: ibm-mq-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-login-api-openapi.yml
- filename: ibm-mq-queue-managers-api-openapi.yml
  format: yaml
  label: IBM MQ Queue Managers API
  slug: ibm-mq-queue-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-queue-managers-api-openapi.yml
- filename: ibm-mq-queue-messaging-api-openapi.yml
  format: yaml
  label: IBM MQ Queue Messaging API
  slug: ibm-mq-queue-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-queue-messaging-api-openapi.yml
- filename: ibm-mq-queues-api-openapi.yml
  format: yaml
  label: IBM MQ Queues API
  slug: ibm-mq-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-queues-api-openapi.yml
- filename: ibm-mq-subscriptions-api-openapi.yml
  format: yaml
  label: IBM MQ Subscriptions API
  slug: ibm-mq-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-subscriptions-api-openapi.yml
- filename: ibm-mq-topic-messaging-api-openapi.yml
  format: yaml
  label: IBM MQ Topic Messaging API
  slug: ibm-mq-topic-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-topic-messaging-api-openapi.yml
- filename: ibm-mq-topics-api-openapi.yml
  format: yaml
  label: IBM MQ Topics API
  slug: ibm-mq-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-topics-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ibm Mq Authentication
name_suffix: Authentication
oauth_flows: []
overview: IBM MQ secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: IBM MQ
provider_slug: ibm-mq
scheme_count: 2
schemes:
- description: HTTP Basic authentication with MQ user credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/ibm-mq-admin-rest-openapi.yml
  - openapi/ibm-mq-messaging-rest-openapi.yml
  type: http
- description: LTPA token-based authentication via login endpoint
  in: cookie
  name: tokenAuth
  parameter: LtpaToken2
  sources:
  - openapi/ibm-mq-admin-rest-openapi.yml
  - openapi/ibm-mq-messaging-rest-openapi.yml
  type: apiKey
slug: ibm-mq-authentication
source_filename: ibm-mq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ibm-mq-admin-rest-openapi.yml, openapi/ibm-mq-messaging-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with MQ user credentials\n  sources:\n  - openapi/ibm-mq-admin-rest-openapi.yml\n  - openapi/ibm-mq-messaging-rest-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: cookie\n  parameter: LtpaToken2\n  description: LTPA token-based authentication via login endpoint\n  sources:\n  - openapi/ibm-mq-admin-rest-openapi.yml\n  - openapi/ibm-mq-messaging-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/authentication/ibm-mq-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Async
- Enterprise
- Integration
- Messaging
- Middleware
- Queue
---
