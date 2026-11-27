---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: la-truite-com-beschikbaarheid-api-openapi.yml
  format: yaml
  label: La Truite d'Argent Beschikbaarheid API
  slug: la-truite-com-beschikbaarheid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/la-truite-com/openapi/la-truite-com-beschikbaarheid-api-openapi.yml
- filename: la-truite-com-boeken-api-openapi.yml
  format: yaml
  label: La Truite d'Argent Boeken API
  slug: la-truite-com-boeken-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/la-truite-com/openapi/la-truite-com-boeken-api-openapi.yml
- filename: la-truite-com-informatie-api-openapi.yml
  format: yaml
  label: La Truite d'Argent Informatie API
  slug: la-truite-com-informatie-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/la-truite-com/openapi/la-truite-com-informatie-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: La Truite d'Argent Authentication
name_suffix: Authentication
oauth_flows: []
overview: La Truite d'Argent secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: La Truite d'Argent
provider_slug: la-truite-com
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/la-truite-com-openapi.json
  type: apiKey
slug: la-truite-com-authentication
source_filename: la-truite-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: derived\nsource: openapi/la-truite-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/la-truite-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/la-truite-com/authentication/la-truite-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Hospitality
- Travel
- Boutique
- RomanticGetaway
- Ardennes
---
