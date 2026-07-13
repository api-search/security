---
api_key_in: []
api_specs:
- filename: onfleet-tasks-api-openapi.yml
  format: yaml
  label: Onfleet Tasks API
  slug: onfleet-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-tasks-api-openapi.yml
- filename: onfleet-workers-api-openapi.yml
  format: yaml
  label: Onfleet Workers API
  slug: onfleet-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-workers-api-openapi.yml
- filename: onfleet-route-plans-api-openapi.yml
  format: yaml
  label: Onfleet Route Plans API
  slug: onfleet-route-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-route-plans-api-openapi.yml
- filename: onfleet-orders-api-openapi.yml
  format: yaml
  label: Onfleet Orders API
  slug: onfleet-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-orders-api-openapi.yml
- filename: onfleet-organizations-api-openapi.yml
  format: yaml
  label: Onfleet Organizations & Teams API
  slug: onfleet-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-organizations-api-openapi.yml
- filename: onfleet-recipients-api-openapi.yml
  format: yaml
  label: Onfleet Recipients API
  slug: onfleet-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-recipients-api-openapi.yml
- filename: onfleet-destinations-api-openapi.yml
  format: yaml
  label: Onfleet Destinations API
  slug: onfleet-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-destinations-api-openapi.yml
- filename: onfleet-webhooks-api-openapi.yml
  format: yaml
  label: Onfleet Webhooks API
  slug: onfleet-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Onfleet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Onfleet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Onfleet
provider_slug: onfleet
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/onfleet-destinations-api-openapi.yml
  - openapi/onfleet-orders-api-openapi.yml
  - openapi/onfleet-organizations-api-openapi.yml
  - openapi/onfleet-recipients-api-openapi.yml
  - openapi/onfleet-route-plans-api-openapi.yml
  - openapi/onfleet-tasks-api-openapi.yml
  - openapi/onfleet-webhooks-api-openapi.yml
  - openapi/onfleet-workers-api-openapi.yml
  type: http
slug: onfleet-authentication
source_filename: onfleet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/onfleet-destinations-api-openapi.yml, openapi/onfleet-orders-api-openapi.yml,\n  openapi/onfleet-organizations-api-openapi.yml, openapi/onfleet-recipients-api-openapi.yml,\n  openapi/onfleet-route-plans-api-openapi.yml, openapi/onfleet-tasks-api-openapi.yml, openapi/onfleet-webhooks-api-openapi.yml,\n  openapi/onfleet-workers-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/onfleet-destinations-api-openapi.yml\n  - openapi/onfleet-orders-api-openapi.yml\n  - openapi/onfleet-organizations-api-openapi.yml\n  - openapi/onfleet-recipients-api-openapi.yml\n  - openapi/onfleet-route-plans-api-openapi.yml\n  - openapi/onfleet-tasks-api-openapi.yml\n  - openapi/onfleet-webhooks-api-openapi.yml\n  - openapi/onfleet-workers-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/authentication/onfleet-authentication.yml
summary_line: http · 1 scheme
tags:
- Last Mile Delivery
- Logistics
- Fleet Management
- Dispatch
- Route Optimization
- Courier
- Drivers
- Tracking
- Geocoding
- Webhooks
- AI
- SaaS
---
