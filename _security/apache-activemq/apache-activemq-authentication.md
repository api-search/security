---
api_key_in: []
api_specs:
- filename: apache-activemq-rest-openapi.yaml
  format: yaml
  label: Apache ActiveMQ REST API
  slug: apache-activemq-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-activemq/refs/heads/main/openapi/apache-activemq-rest-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Activemq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache ActiveMQ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache ActiveMQ
provider_slug: apache-activemq
scheme_count: 1
schemes:
- description: HTTP Basic authentication using broker credentials. Default credentials are admin/admin but should be changed in production via jetty-realm.properties.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-activemq-rest-openapi.yaml
  type: http
slug: apache-activemq-authentication
source_filename: apache-activemq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-activemq-rest-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using broker credentials. Default credentials are admin/admin\n    but should be changed in production via jetty-realm.properties.\n  sources:\n  - openapi/apache-activemq-rest-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-activemq/refs/heads/main/authentication/apache-activemq-authentication.yml
summary_line: http · 1 scheme
tags:
- AMQP
- Apache
- Java
- JMS
- Message Broker
- Messaging
- MQTT
- Open Source
- STOMP
---
