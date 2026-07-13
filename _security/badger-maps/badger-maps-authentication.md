---
api_key_in:
- header
api_specs:
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Accounts API
  slug: badger-maps-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Locations API
  slug: badger-maps-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Check-Ins API
  slug: badger-maps-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Routes API
  slug: badger-maps-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
- filename: badger-maps-openapi.yml
  format: yaml
  label: Badger Maps Users API
  slug: badger-maps-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/openapi/badger-maps-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Badger Maps Authentication
name_suffix: Authentication
oauth_flows: []
overview: Badger Maps secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Badger Maps
provider_slug: badger-maps
scheme_count: 1
schemes:
- description: 'Token authentication. Send `Authorization: Token <api_key>`. Contact Badger Maps support to have your API/Developer Key enabled.'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/badger-maps-openapi.yml
  type: apiKey
slug: badger-maps-authentication
source_filename: badger-maps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/badger-maps-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token authentication. Send `Authorization: Token <api_key>`. Contact Badger\n    Maps support to have your API/Developer Key enabled.'\n  sources:\n  - openapi/badger-maps-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/badger-maps/refs/heads/main/authentication/badger-maps-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Field Sales
- Route Planning
- Mapping
- CRM
- Sales Enablement
- Territory Management
---
