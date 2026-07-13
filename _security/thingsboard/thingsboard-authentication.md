---
api_key_in:
- header
api_specs:
- filename: thingsboard-devices-openapi.yml
  format: yaml
  label: ThingsBoard Devices API
  slug: thingsboard-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-devices-openapi.yml
- filename: thingsboard-assets-openapi.yml
  format: yaml
  label: ThingsBoard Assets API
  slug: thingsboard-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-assets-openapi.yml
- filename: thingsboard-telemetry-openapi.yml
  format: yaml
  label: ThingsBoard Telemetry API
  slug: thingsboard-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-telemetry-openapi.yml
- filename: thingsboard-alarms-openapi.yml
  format: yaml
  label: ThingsBoard Alarms API
  slug: thingsboard-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-alarms-openapi.yml
- filename: thingsboard-rule-engine-openapi.yml
  format: yaml
  label: ThingsBoard Rule Engine API
  slug: thingsboard-rule-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-rule-engine-openapi.yml
- filename: thingsboard-rpc-openapi.yml
  format: yaml
  label: ThingsBoard RPC API
  slug: thingsboard-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-rpc-openapi.yml
- filename: thingsboard-dashboards-openapi.yml
  format: yaml
  label: ThingsBoard Dashboards API
  slug: thingsboard-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-dashboards-openapi.yml
- filename: thingsboard-auth-openapi.yml
  format: yaml
  label: ThingsBoard Authentication API
  slug: thingsboard-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-auth-openapi.yml
- filename: thingsboard-tenants-openapi.yml
  format: yaml
  label: ThingsBoard Tenants and Customers API
  slug: thingsboard-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-tenants-openapi.yml
- filename: thingsboard-admin-openapi.yml
  format: yaml
  label: ThingsBoard Admin API
  slug: thingsboard-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-admin-openapi.yml
- filename: thingsboard-notifications-openapi.yml
  format: yaml
  label: ThingsBoard Notifications API
  slug: thingsboard-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-notifications-openapi.yml
- filename: thingsboard-edge-openapi.yml
  format: yaml
  label: ThingsBoard Edge API
  slug: thingsboard-edge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-edge-openapi.yml
- filename: thingsboard-mobile-openapi.yml
  format: yaml
  label: ThingsBoard Mobile App API
  slug: thingsboard-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-mobile-openapi.yml
- filename: thingsboard-lwm2m-openapi.yml
  format: yaml
  label: ThingsBoard LwM2M API
  slug: thingsboard-lwm2m-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-lwm2m-openapi.yml
- filename: thingsboard-ai-openapi.yml
  format: yaml
  label: ThingsBoard AI API
  slug: thingsboard-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-ai-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Thingsboard Authentication
name_suffix: Authentication
oauth_flows: []
overview: ThingsBoard secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ThingsBoard
provider_slug: thingsboard
scheme_count: 2
schemes:
- bearerFormat: /api/auth/login|X-Authorization
  description: Enter Username / Password
  name: HTTP login form
  scheme: loginPassword
  sources:
  - openapi/thingsboard-admin-openapi.yml
  - openapi/thingsboard-ai-openapi.yml
  - openapi/thingsboard-alarms-openapi.yml
  - openapi/thingsboard-assets-openapi.yml
  - openapi/thingsboard-auth-openapi.yml
  - openapi/thingsboard-dashboards-openapi.yml
  - openapi/thingsboard-devices-openapi.yml
  - openapi/thingsboard-edge-openapi.yml
  - openapi/thingsboard-lwm2m-openapi.yml
  - openapi/thingsboard-mobile-openapi.yml
  - openapi/thingsboard-notifications-openapi.yml
  - openapi/thingsboard-rpc-openapi.yml
  - openapi/thingsboard-rule-engine-openapi.yml
  - openapi/thingsboard-telemetry-openapi.yml
  - openapi/thingsboard-tenants-openapi.yml
  type: http
- description: 'Enter the API key value with ''ApiKey'' prefix in format: **ApiKey <your_api_key_value>**


    Example: **ApiKey tb_5te51SkLRYpjGrujUGwqkjFvooWBlQpVe2An2Dr3w13wjfxDW**


    <br>**NOTE**: Use only ONE authentication method at a time. If both are authorized, JWT auth takes the priority.<br>'
  in: header
  name: API key form
  parameter: X-Authorization
  sources:
  - openapi/thingsboard-admin-openapi.yml
  - openapi/thingsboard-ai-openapi.yml
  - openapi/thingsboard-alarms-openapi.yml
  - openapi/thingsboard-assets-openapi.yml
  - openapi/thingsboard-auth-openapi.yml
  - openapi/thingsboard-dashboards-openapi.yml
  - openapi/thingsboard-devices-openapi.yml
  - openapi/thingsboard-edge-openapi.yml
  - openapi/thingsboard-lwm2m-openapi.yml
  - openapi/thingsboard-mobile-openapi.yml
  - openapi/thingsboard-notifications-openapi.yml
  - openapi/thingsboard-rpc-openapi.yml
  - openapi/thingsboard-rule-engine-openapi.yml
  - openapi/thingsboard-telemetry-openapi.yml
  - openapi/thingsboard-tenants-openapi.yml
  type: apiKey
slug: thingsboard-authentication
source_filename: thingsboard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thingsboard-admin-openapi.yml, openapi/thingsboard-ai-openapi.yml, openapi/thingsboard-alarms-openapi.yml,\n  openapi/thingsboard-assets-openapi.yml, openapi/thingsboard-auth-openapi.yml, openapi/thingsboard-dashboards-openapi.yml,\n  openapi/thingsboard-devices-openapi.yml, openapi/thingsboard-edge-openapi.yml, openapi/thingsboard-lwm2m-openapi.yml,\n  openapi/thingsboard-mobile-openapi.yml, openapi/thingsboard-notifications-openapi.yml, openapi/thingsboard-rpc-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: HTTP login form\n  type: http\n  scheme: loginPassword\n  bearerFormat: /api/auth/login|X-Authorization\n  description: Enter Username / Password\n  sources:\n  - openapi/thingsboard-admin-openapi.yml\n  - openapi/thingsboard-ai-openapi.yml\n  - openapi/thingsboard-alarms-openapi.yml\n  - openapi/thingsboard-assets-openapi.yml\n  - openapi/thingsboard-auth-openapi.yml\n\
  \  - openapi/thingsboard-dashboards-openapi.yml\n  - openapi/thingsboard-devices-openapi.yml\n  - openapi/thingsboard-edge-openapi.yml\n  - openapi/thingsboard-lwm2m-openapi.yml\n  - openapi/thingsboard-mobile-openapi.yml\n  - openapi/thingsboard-notifications-openapi.yml\n  - openapi/thingsboard-rpc-openapi.yml\n  - openapi/thingsboard-rule-engine-openapi.yml\n  - openapi/thingsboard-telemetry-openapi.yml\n  - openapi/thingsboard-tenants-openapi.yml\n- name: API key form\n  type: apiKey\n  in: header\n  parameter: X-Authorization\n  description: |-\n    Enter the API key value with 'ApiKey' prefix in format: **ApiKey <your_api_key_value>**\n\n    Example: **ApiKey tb_5te51SkLRYpjGrujUGwqkjFvooWBlQpVe2An2Dr3w13wjfxDW**\n\n    <br>**NOTE**: Use only ONE authentication method at a time. If both are authorized, JWT auth takes the priority.<br>\n  sources:\n  - openapi/thingsboard-admin-openapi.yml\n  - openapi/thingsboard-ai-openapi.yml\n  - openapi/thingsboard-alarms-openapi.yml\n  - openapi/thingsboard-assets-openapi.yml\n\
  \  - openapi/thingsboard-auth-openapi.yml\n  - openapi/thingsboard-dashboards-openapi.yml\n  - openapi/thingsboard-devices-openapi.yml\n  - openapi/thingsboard-edge-openapi.yml\n  - openapi/thingsboard-lwm2m-openapi.yml\n  - openapi/thingsboard-mobile-openapi.yml\n  - openapi/thingsboard-notifications-openapi.yml\n  - openapi/thingsboard-rpc-openapi.yml\n  - openapi/thingsboard-rule-engine-openapi.yml\n  - openapi/thingsboard-telemetry-openapi.yml\n  - openapi/thingsboard-tenants-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/authentication/thingsboard-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- IoT
- Internet of Things
- Device Management
- Telemetry
- Open Source
- Apache 2.0
- MQTT
- LwM2M
- CoAP
- Rule Engine
- Dashboards
- Edge
- Multi-tenant
- Java
- Spring
---
