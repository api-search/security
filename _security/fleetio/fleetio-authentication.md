---
api_key_in:
- header
api_specs:
- filename: fleetio-contacts-api-openapi.yml
  format: yaml
  label: Fleetio Contacts API
  slug: fleetio-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-contacts-api-openapi.yml
- filename: fleetio-fuel-entries-api-openapi.yml
  format: yaml
  label: Fleetio Fuel Entries API
  slug: fleetio-fuel-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-fuel-entries-api-openapi.yml
- filename: fleetio-inspections-api-openapi.yml
  format: yaml
  label: Fleetio Inspections API
  slug: fleetio-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-inspections-api-openapi.yml
- filename: fleetio-inventory-journal-entries-api-openapi.yml
  format: yaml
  label: Fleetio Inventory Journal Entries API
  slug: fleetio-inventory-journal-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-inventory-journal-entries-api-openapi.yml
- filename: fleetio-issues-api-openapi.yml
  format: yaml
  label: Fleetio Issues API
  slug: fleetio-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-issues-api-openapi.yml
- filename: fleetio-parts-api-openapi.yml
  format: yaml
  label: Fleetio Parts API
  slug: fleetio-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-parts-api-openapi.yml
- filename: fleetio-service-entries-api-openapi.yml
  format: yaml
  label: Fleetio Service Entries API
  slug: fleetio-service-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-service-entries-api-openapi.yml
- filename: fleetio-service-reminders-api-openapi.yml
  format: yaml
  label: Fleetio Service Reminders API
  slug: fleetio-service-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-service-reminders-api-openapi.yml
- filename: fleetio-vehicles-api-openapi.yml
  format: yaml
  label: Fleetio Vehicles API
  slug: fleetio-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-vehicles-api-openapi.yml
- filename: fleetio-webhooks-api-openapi.yml
  format: yaml
  label: Fleetio Webhooks API
  slug: fleetio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-webhooks-api-openapi.yml
- filename: fleetio-work-orders-api-openapi.yml
  format: yaml
  label: Fleetio Work Orders API
  slug: fleetio-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-work-orders-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fleetio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fleetio secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fleetio
provider_slug: fleetio
scheme_count: 2
schemes:
- description: 'API key associated with a Fleetio user, prefixed with the word "Token" (e.g. "Authorization: Token YOUR_API_KEY"). Generate keys at https://secure.fleetio.com/api_keys.'
  in: header
  name: AuthorizationToken
  parameter: Authorization
  sources:
  - openapi/fleetio-openapi.yml
  type: apiKey
- description: Account token identifying the Fleetio account.
  in: header
  name: AccountToken
  parameter: Account-Token
  sources:
  - openapi/fleetio-openapi.yml
  type: apiKey
slug: fleetio-authentication
source_filename: fleetio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fleetio-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AuthorizationToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key associated with a Fleetio user, prefixed with the word \"Token\" (e.g.\n    \"Authorization: Token YOUR_API_KEY\"). Generate keys at https://secure.fleetio.com/api_keys.'\n  sources:\n  - openapi/fleetio-openapi.yml\n- name: AccountToken\n  type: apiKey\n  in: header\n  parameter: Account-Token\n  description: Account token identifying the Fleetio account.\n  sources:\n  - openapi/fleetio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/authentication/fleetio-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Fleet Management
- Vehicles
- Maintenance
- Telematics
- SaaS
---
