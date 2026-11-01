---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: geospatialsystem-com-catalogue-api-openapi.yml
  format: yaml
  label: geospatialsystem-com Catalogue API
  slug: geospatialsystem-com-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geospatialsystem-com/openapi/geospatialsystem-com-catalogue-api-openapi.yml
- filename: geospatialsystem-com-level-1-pixel-api-openapi.yml
  format: yaml
  label: geospatialsystem-com Level 1 — Pixel API
  slug: geospatialsystem-com-level-1-pixel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geospatialsystem-com/openapi/geospatialsystem-com-level-1-pixel-api-openapi.yml
- filename: geospatialsystem-com-level-2-neighbourhood-api-openapi.yml
  format: yaml
  label: geospatialsystem-com Level 2 — Neighbourhood API
  slug: geospatialsystem-com-level-2-neighbourhood-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geospatialsystem-com/openapi/geospatialsystem-com-level-2-neighbourhood-api-openapi.yml
- filename: geospatialsystem-com-level-3-area-maps-api-openapi.yml
  format: yaml
  label: geospatialsystem-com Level 3 — Area Maps API
  slug: geospatialsystem-com-level-3-area-maps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geospatialsystem-com/openapi/geospatialsystem-com-level-3-area-maps-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Geospatialsystem Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: geospatialsystem-com secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: geospatialsystem-com
provider_slug: geospatialsystem-com
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/geospatialsystem-com-openapi.json
  type: apiKey
slug: geospatialsystem-com-authentication
source_filename: geospatialsystem-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/geospatialsystem-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/geospatialsystem-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/geospatialsystem-com/authentication/geospatialsystem-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Geospatial
- Terrain
- API
- AI
- Location
---
