---
api_key_in:
- header
api_specs:
- filename: hildebrand-glowmarkt-user-system-swagger.json
  format: json
  label: Glowmarkt User System API
  slug: glowmarkt-user-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hildebrand/refs/heads/main/openapi/hildebrand-glowmarkt-user-system-swagger.json
- filename: hildebrand-glowmarkt-resource-system-swagger.json
  format: json
  label: Glowmarkt Resource System API
  slug: glowmarkt-resource-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hildebrand/refs/heads/main/openapi/hildebrand-glowmarkt-resource-system-swagger.json
- filename: hildebrand-glowmarkt-virtual-entity-system-swagger.json
  format: json
  label: Glowmarkt Virtual Entity System API
  slug: glowmarkt-virtual-entity-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hildebrand/refs/heads/main/openapi/hildebrand-glowmarkt-virtual-entity-system-swagger.json
- filename: hildebrand-glowmarkt-device-management-system-swagger.json
  format: json
  label: Glowmarkt Device Management System API
  slug: glowmarkt-device-management-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hildebrand/refs/heads/main/openapi/hildebrand-glowmarkt-device-management-system-swagger.json
- filename: hildebrand-glowmarkt-notification-system-swagger.json
  format: json
  label: Glowmarkt Notification System API
  slug: glowmarkt-notification-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hildebrand/refs/heads/main/openapi/hildebrand-glowmarkt-notification-system-swagger.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hildebrand Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hildebrand secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hildebrand
provider_slug: hildebrand
scheme_count: 5
schemes:
- name: orgAppKeys
  scheme: basic
  sources:
  - openapi/hildebrand-glowmarkt-device-management-system-swagger.json
  - openapi/hildebrand-glowmarkt-notification-system-swagger.json
  - openapi/hildebrand-glowmarkt-resource-system-swagger.json
  - openapi/hildebrand-glowmarkt-user-system-swagger.json
  - openapi/hildebrand-glowmarkt-virtual-entity-system-swagger.json
  type: http
- in: header
  name: devUserToken
  parameter: token
  sources:
  - openapi/hildebrand-glowmarkt-device-management-system-swagger.json
  - openapi/hildebrand-glowmarkt-notification-system-swagger.json
  - openapi/hildebrand-glowmarkt-resource-system-swagger.json
  - openapi/hildebrand-glowmarkt-user-system-swagger.json
  - openapi/hildebrand-glowmarkt-virtual-entity-system-swagger.json
  type: apiKey
- in: header
  name: applicationId
  parameter: applicationId
  sources:
  - openapi/hildebrand-glowmarkt-device-management-system-swagger.json
  - openapi/hildebrand-glowmarkt-notification-system-swagger.json
  - openapi/hildebrand-glowmarkt-resource-system-swagger.json
  - openapi/hildebrand-glowmarkt-user-system-swagger.json
  - openapi/hildebrand-glowmarkt-virtual-entity-system-swagger.json
  type: apiKey
- in: header
  name: userId
  parameter: userId
  sources:
  - openapi/hildebrand-glowmarkt-device-management-system-swagger.json
  - openapi/hildebrand-glowmarkt-resource-system-swagger.json
  - openapi/hildebrand-glowmarkt-user-system-swagger.json
  type: apiKey
- in: header
  name: organizationId
  parameter: organizationId
  sources:
  - openapi/hildebrand-glowmarkt-notification-system-swagger.json
  - openapi/hildebrand-glowmarkt-user-system-swagger.json
  type: apiKey
slug: hildebrand-authentication
source_filename: hildebrand-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/hildebrand-glowmarkt-device-management-system-swagger.json, openapi/hildebrand-glowmarkt-notification-system-swagger.json,\n  openapi/hildebrand-glowmarkt-resource-system-swagger.json, openapi/hildebrand-glowmarkt-user-system-swagger.json,\n  openapi/hildebrand-glowmarkt-virtual-entity-system-swagger.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: orgAppKeys\n  type: http\n  scheme: basic\n  sources:\n  - openapi/hildebrand-glowmarkt-device-management-system-swagger.json\n  - openapi/hildebrand-glowmarkt-notification-system-swagger.json\n  - openapi/hildebrand-glowmarkt-resource-system-swagger.json\n  - openapi/hildebrand-glowmarkt-user-system-swagger.json\n  - openapi/hildebrand-glowmarkt-virtual-entity-system-swagger.json\n- name: devUserToken\n  type: apiKey\n  in: header\n  parameter: token\n  sources:\n  - openapi/hildebrand-glowmarkt-device-management-system-swagger.json\n\
  \  - openapi/hildebrand-glowmarkt-notification-system-swagger.json\n  - openapi/hildebrand-glowmarkt-resource-system-swagger.json\n  - openapi/hildebrand-glowmarkt-user-system-swagger.json\n  - openapi/hildebrand-glowmarkt-virtual-entity-system-swagger.json\n- name: applicationId\n  type: apiKey\n  in: header\n  parameter: applicationId\n  sources:\n  - openapi/hildebrand-glowmarkt-device-management-system-swagger.json\n  - openapi/hildebrand-glowmarkt-notification-system-swagger.json\n  - openapi/hildebrand-glowmarkt-resource-system-swagger.json\n  - openapi/hildebrand-glowmarkt-user-system-swagger.json\n  - openapi/hildebrand-glowmarkt-virtual-entity-system-swagger.json\n- name: userId\n  type: apiKey\n  in: header\n  parameter: userId\n  sources:\n  - openapi/hildebrand-glowmarkt-device-management-system-swagger.json\n  - openapi/hildebrand-glowmarkt-resource-system-swagger.json\n  - openapi/hildebrand-glowmarkt-user-system-swagger.json\n- name: organizationId\n  type: apiKey\n  in:\
  \ header\n  parameter: organizationId\n  sources:\n  - openapi/hildebrand-glowmarkt-notification-system-swagger.json\n  - openapi/hildebrand-glowmarkt-user-system-swagger.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hildebrand/refs/heads/main/authentication/hildebrand-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Energy Data
- Demand Response
- IoT
- Metering
---
