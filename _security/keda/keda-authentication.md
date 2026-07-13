---
api_key_in:
- header
api_specs:
- filename: keda-metrics-api-openapi.yml
  format: yaml
  label: KEDA Metrics API
  slug: keda-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keda/refs/heads/main/openapi/keda-metrics-api-openapi.yml
- filename: keda-cloud-events-asyncapi.yml
  format: yaml
  label: KEDA CloudEventSource API
  slug: keda-cloud-event-source-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/keda/refs/heads/main/asyncapi/keda-cloud-events-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Keda Authentication
name_suffix: Authentication
oauth_flows: []
overview: KEDA secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: KEDA
provider_slug: keda
scheme_count: 3
schemes:
- description: Bearer token authentication for secured metrics endpoints.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/keda-metrics-api-openapi.yml
  type: http
- description: Basic authentication for secured metrics endpoints.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/keda-metrics-api-openapi.yml
  type: http
- description: API key authentication via header for secured metrics endpoints.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/keda-metrics-api-openapi.yml
  type: apiKey
slug: keda-authentication
source_filename: keda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keda-metrics-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication for secured metrics endpoints.\n  sources:\n  - openapi/keda-metrics-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication for secured metrics endpoints.\n  sources:\n  - openapi/keda-metrics-api-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key authentication via header for secured metrics endpoints.\n  sources:\n  - openapi/keda-metrics-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keda/refs/heads/main/authentication/keda-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Autoscaling
- CNCF
- Event-Driven
- Graduated
- Kubernetes
---
