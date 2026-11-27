---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: la-palma24-net-precios-api-openapi.yml
  format: yaml
  label: La Palma 24 Precios API
  slug: la-palma24-net-precios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/la-palma24-net/openapi/la-palma24-net-precios-api-openapi.yml
- filename: la-palma24-net-propiedades-api-openapi.yml
  format: yaml
  label: La Palma 24 Propiedades API
  slug: la-palma24-net-propiedades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/la-palma24-net/openapi/la-palma24-net-propiedades-api-openapi.yml
- filename: la-palma24-net-ubicaciones-api-openapi.yml
  format: yaml
  label: La Palma 24 Ubicaciones API
  slug: la-palma24-net-ubicaciones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/la-palma24-net/openapi/la-palma24-net-ubicaciones-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: La Palma 24 Authentication
name_suffix: Authentication
oauth_flows: []
overview: La Palma 24 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: La Palma 24
provider_slug: la-palma24-net
scheme_count: 1
schemes:
- description: API Key para autenticación
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/la-palma24-net-openapi.json
  type: apiKey
slug: la-palma24-net-authentication
source_filename: la-palma24-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: derived\nsource: openapi/la-palma24-net-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API Key para autenticación\n  sources:\n  - openapi/la-palma24-net-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/la-palma24-net/authentication/la-palma24-net-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Vacation Rentals
- Travel
- Spain
- La Palma
- Hospitality
---
