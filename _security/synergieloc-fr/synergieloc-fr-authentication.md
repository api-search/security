---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: synergieloc-fr-acquisition-api-openapi.yml
  format: yaml
  label: Synergieloc Acquisition API
  slug: synergieloc-fr-acquisition-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synergieloc-fr/openapi/synergieloc-fr-acquisition-api-openapi.yml
- filename: synergieloc-fr-api-ia-api-openapi.yml
  format: yaml
  label: Synergieloc API Ia API
  slug: synergieloc-fr-api-ia-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synergieloc-fr/openapi/synergieloc-fr-api-ia-api-openapi.yml
- filename: synergieloc-fr-api-ia-industrial-api-openapi.yml
  format: yaml
  label: Synergieloc API Ia Industrial API
  slug: synergieloc-fr-api-ia-industrial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synergieloc-fr/openapi/synergieloc-fr-api-ia-industrial-api-openapi.yml
- filename: synergieloc-fr-cao-indus-api-openapi.yml
  format: yaml
  label: Synergieloc Cao Indus API
  slug: synergieloc-fr-cao-indus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synergieloc-fr/openapi/synergieloc-fr-cao-indus-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Synergieloc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synergieloc secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Synergieloc
provider_slug: synergieloc-fr
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/synergieloc-fr-openapi.json
  type: apiKey
slug: synergieloc-fr-authentication
source_filename: synergieloc-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: derived\nsource: openapi/synergieloc-fr-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/synergieloc-fr-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/synergieloc-fr/authentication/synergieloc-fr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- RealEstate
- SaaS
- PropertyManagement
- Rental
---
