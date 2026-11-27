---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: mercantry-org-bookings-api-openapi.yml
  format: yaml
  label: Mercantry Bookings API
  slug: mercantry-org-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mercantry-org/openapi/mercantry-org-bookings-api-openapi.yml
- filename: mercantry-org-export-api-openapi.yml
  format: yaml
  label: Mercantry Export API
  slug: mercantry-org-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mercantry-org/openapi/mercantry-org-export-api-openapi.yml
- filename: mercantry-org-healthz-api-openapi.yml
  format: yaml
  label: Mercantry Healthz API
  slug: mercantry-org-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mercantry-org/openapi/mercantry-org-healthz-api-openapi.yml
- filename: mercantry-org-keys-api-openapi.yml
  format: yaml
  label: Mercantry Keys API
  slug: mercantry-org-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mercantry-org/openapi/mercantry-org-keys-api-openapi.yml
- filename: mercantry-org-merchants-api-openapi.yml
  format: yaml
  label: Mercantry Merchants API
  slug: mercantry-org-merchants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mercantry-org/openapi/mercantry-org-merchants-api-openapi.yml
- filename: mercantry-org-meta-api-openapi.yml
  format: yaml
  label: Mercantry Meta API
  slug: mercantry-org-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mercantry-org/openapi/mercantry-org-meta-api-openapi.yml
- filename: mercantry-org-stats-api-openapi.yml
  format: yaml
  label: Mercantry Stats API
  slug: mercantry-org-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mercantry-org/openapi/mercantry-org-stats-api-openapi.yml
- filename: mercantry-org-well-known-api-openapi.yml
  format: yaml
  label: Mercantry .well Known API
  slug: mercantry-org-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mercantry-org/openapi/mercantry-org-well-known-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Mercantry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mercantry secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mercantry
provider_slug: mercantry-org
scheme_count: 1
schemes:
- description: 'Optional developer key from POST /v1/keys. Also accepted as Authorization: Bearer <key>.'
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/mercantry-org-openapi.json
  type: apiKey
slug: mercantry-org-authentication
source_filename: mercantry-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mercantry-org-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Optional developer key from POST /v1/keys. Also accepted as Authorization: Bearer\n    <key>.'\n  sources:\n  - openapi/mercantry-org-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mercantry-org/authentication/mercantry-org-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Commerce Registry
- AI Agents
- Merchant Data
- Booking Fulfillment
- Open Data
---
