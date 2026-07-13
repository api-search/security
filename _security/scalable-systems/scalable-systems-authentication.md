---
api_key_in:
- header
api_specs:
- filename: haproxy_spec.yaml
  format: yaml
  label: HAProxy Data Plane API
  slug: haproxy
  spec_type: OpenAPI
  url: https://github.com/haproxytech/dataplaneapi/blob/master/specification/build/haproxy_spec.yaml
- filename: management-api.json
  format: json
  label: RabbitMQ Management API
  slug: rabbitmq
  spec_type: OpenAPI
  url: https://www.rabbitmq.com/resources/specs/management-api.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scalable Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scalable Systems secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scalable Systems
provider_slug: scalable-systems
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed request (Authorization header).
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/scalable-systems-openapi.yml
  type: apiKey
slug: scalable-systems-authentication
source_filename: scalable-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scalable-systems-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed request (Authorization header).\n  sources:\n  - openapi/scalable-systems-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-systems/refs/heads/main/authentication/scalable-systems-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Auto Scaling
- Caching
- Cloud Infrastructure
- Distributed Systems
- High Availability
- Infrastructure
- Load Balancing
- Message Queues
- Platform Engineering
- Scalable Architecture
- Service Discovery
---
