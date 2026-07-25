---
api_key_in: []
api_specs:
- filename: bmw-connecteddrive-containers-api-openapi.yml
  format: yaml
  label: BMW ConnectedDrive Containers API
  slug: bmw-connecteddrive-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmw-connecteddrive/refs/heads/main/openapi/bmw-connecteddrive-containers-api-openapi.yml
- filename: bmw-connecteddrive-vehicles-api-openapi.yml
  format: yaml
  label: BMW ConnectedDrive Vehicles API
  slug: bmw-connecteddrive-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmw-connecteddrive/refs/heads/main/openapi/bmw-connecteddrive-vehicles-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bmw Connecteddrive Authentication
name_suffix: Authentication
oauth_flows: []
overview: BMW ConnectedDrive secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BMW ConnectedDrive
provider_slug: bmw-connecteddrive
scheme_count: 1
schemes:
- bearerFormat: opaque
  description: GCDM Access Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bmw-cardata-customer-api-openapi.json
  type: http
slug: bmw-connecteddrive-authentication
source_filename: bmw-connecteddrive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bmw-cardata-customer-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  description: GCDM Access Token\n  sources:\n  - openapi/bmw-cardata-customer-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bmw-connecteddrive/refs/heads/main/authentication/bmw-connecteddrive-authentication.yml
summary_line: http · 1 scheme
tags:
- Automotive
- Connected Vehicle
- Telematics
- Vehicle Data
- CarData
- ConnectedDrive
- Electric Vehicles
- Charging
- MQTT
- Streaming
- OAuth
- Device Code Flow
- GDPR
- Right To Repair
- Mobility
---
