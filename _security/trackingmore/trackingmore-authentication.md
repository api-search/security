---
api_key_in:
- header
api_specs:
- filename: trackingmore-openapi.yml
  format: yaml
  label: TrackingMore API
  slug: trackingmore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trackingmore/refs/heads/main/openapi/trackingmore-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trackingmore Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrackingMore secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TrackingMore
provider_slug: trackingmore
scheme_count: 1
schemes:
- description: API key for authentication. Obtainable from your TrackingMore account dashboard. Up to 4 API keys per account.
  in: header
  name: ApiKeyAuth
  parameter: Tracking-Api-Key
  sources:
  - openapi/trackingmore-openapi.yml
  type: apiKey
slug: trackingmore-authentication
source_filename: trackingmore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trackingmore-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Tracking-Api-Key\n  description: API key for authentication. Obtainable from your TrackingMore account dashboard.\n    Up to 4 API keys per account.\n  sources:\n  - openapi/trackingmore-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trackingmore/refs/heads/main/authentication/trackingmore-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Logistics
- Shipping
- Tracking
- Parcels
- Webhooks
- Ecommerce
---
