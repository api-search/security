---
api_key_in:
- header
api_specs:
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Vehicles API
  slug: vehicles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Contacts API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Fuel Entries API
  slug: fuel-entries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Service & Work Orders API
  slug: service-work-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Parts & Inventory API
  slug: parts-inventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Inspections API
  slug: inspections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Issues API
  slug: issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
- filename: fleetio-openapi.yml
  format: yaml
  label: Fleetio Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetio/refs/heads/main/openapi/fleetio-openapi.yml
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
