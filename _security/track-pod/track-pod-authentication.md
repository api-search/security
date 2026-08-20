---
api_key_in:
- header
api_specs:
- filename: track-pod-address-api-openapi.yml
  format: yaml
  label: Track-POD Address API
  slug: track-pod-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/track-pod/refs/heads/main/openapi/track-pod-address-api-openapi.yml
- filename: track-pod-driver-api-openapi.yml
  format: yaml
  label: Track-POD Driver API
  slug: track-pod-driver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/track-pod/refs/heads/main/openapi/track-pod-driver-api-openapi.yml
- filename: track-pod-order-api-openapi.yml
  format: yaml
  label: Track-POD Order API
  slug: track-pod-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/track-pod/refs/heads/main/openapi/track-pod-order-api-openapi.yml
- filename: track-pod-rejectreason-api-openapi.yml
  format: yaml
  label: Track-POD RejectReason API
  slug: track-pod-rejectreason-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/track-pod/refs/heads/main/openapi/track-pod-rejectreason-api-openapi.yml
- filename: track-pod-route-api-openapi.yml
  format: yaml
  label: Track-POD Route API
  slug: track-pod-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/track-pod/refs/heads/main/openapi/track-pod-route-api-openapi.yml
- filename: track-pod-test-api-openapi.yml
  format: yaml
  label: Track-POD Test API
  slug: track-pod-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/track-pod/refs/heads/main/openapi/track-pod-test-api-openapi.yml
- filename: track-pod-vehicle-api-openapi.yml
  format: yaml
  label: Track-POD Vehicle API
  slug: track-pod-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/track-pod/refs/heads/main/openapi/track-pod-vehicle-api-openapi.yml
- filename: track-pod-vehiclecheck-api-openapi.yml
  format: yaml
  label: Track-POD VehicleCheck API
  slug: track-pod-vehiclecheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/track-pod/refs/heads/main/openapi/track-pod-vehiclecheck-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Track Pod Authentication
name_suffix: Authentication
oauth_flows: []
overview: Track-POD secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Track-POD
provider_slug: track-pod
scheme_count: 1
schemes:
- description: Please enter API key into field
  in: header
  name: ApiKey
  parameter: X-API-KEY
  sources:
  - openapi/track-pod-openapi.yml
  type: apiKey
slug: track-pod-authentication
source_filename: track-pod-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/track-pod-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Please enter API key into field\n  sources:\n  - openapi/track-pod-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/track-pod/refs/heads/main/authentication/track-pod-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Delivery
- Last Mile
- Logistics
- Proof of Delivery
- Electronic Proof Of Delivery
- EPOD
- Route Planning
- Route Optimization
- Dispatch
- Fleet Management
- Driver Tracking
- Couriers
- Field Service
- Transportation
- Shipping
---
