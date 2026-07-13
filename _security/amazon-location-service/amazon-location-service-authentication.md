---
api_key_in:
- header
api_specs:
- filename: amazon-location-service-openapi.yml
  format: yaml
  label: Amazon Location Service REST API
  slug: amazon-location-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-location-service/refs/heads/main/openapi/amazon-location-service-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Location Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Location Service secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Location Service
provider_slug: amazon-location-service
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-location-service-openapi.yml
  type: apiKey
slug: amazon-location-service-authentication
source_filename: amazon-location-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-location-service-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-location-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-location-service/refs/heads/main/authentication/amazon-location-service-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Geocoding
- Geofencing
- Location
- Maps
- Routing
---
