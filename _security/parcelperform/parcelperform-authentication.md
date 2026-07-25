---
api_key_in: []
api_specs:
- filename: parcelperform-analytics-api-openapi.yml
  format: yaml
  label: Parcel Perform Analytics API
  slug: parcelperform-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-analytics-api-openapi.yml
- filename: parcelperform-authentication-api-openapi.yml
  format: yaml
  label: Parcel Perform Authentication API
  slug: parcelperform-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-authentication-api-openapi.yml
- filename: parcelperform-couriers-api-openapi.yml
  format: yaml
  label: Parcel Perform Couriers API
  slug: parcelperform-couriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-couriers-api-openapi.yml
- filename: parcelperform-returns-api-openapi.yml
  format: yaml
  label: Parcel Perform Returns API
  slug: parcelperform-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-returns-api-openapi.yml
- filename: parcelperform-shipments-api-openapi.yml
  format: yaml
  label: Parcel Perform Shipments API
  slug: parcelperform-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-shipments-api-openapi.yml
- filename: parcelperform-tracking-events-api-openapi.yml
  format: yaml
  label: Parcel Perform Tracking Events API
  slug: parcelperform-tracking-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-tracking-events-api-openapi.yml
- filename: parcelperform-webhooks-api-openapi.yml
  format: yaml
  label: Parcel Perform Webhooks API
  slug: parcelperform-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Parcelperform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parcel Perform secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parcel Perform
provider_slug: parcelperform
scheme_count: 1
schemes:
- description: 'Bearer access token obtained from POST /auth/oauth/token/, valid for 3600 seconds (60 minutes) per indexed integration guides. Passed as `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/parcelperform-openapi.yml
  type: http
slug: parcelperform-authentication
source_filename: parcelperform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parcelperform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer access token obtained from POST /auth/oauth/token/, valid for 3600 seconds\n    (60 minutes) per indexed integration guides. Passed as `Authorization: Bearer [example key]`.'\n  sources:\n  - openapi/parcelperform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/authentication/parcelperform-authentication.yml
summary_line: http · 1 scheme
tags:
- Logistics
- Shipment Tracking
- Post-Purchase
- Delivery Experience
- Returns
- E-Commerce
---
