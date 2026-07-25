---
api_key_in:
- query
api_specs:
- filename: constellation-brands-bottleshots-api-openapi.yml
  format: yaml
  label: Constellation Brands BottleShots API
  slug: constellation-brands-bottleshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-bottleshots-api-openapi.yml
- filename: constellation-brands-hotsheets-api-openapi.yml
  format: yaml
  label: Constellation Brands HotSheets API
  slug: constellation-brands-hotsheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-hotsheets-api-openapi.yml
- filename: constellation-brands-items-api-openapi.yml
  format: yaml
  label: Constellation Brands Items API
  slug: constellation-brands-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-items-api-openapi.yml
- filename: constellation-brands-neckhangers-api-openapi.yml
  format: yaml
  label: Constellation Brands NeckHangers API
  slug: constellation-brands-neckhangers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-neckhangers-api-openapi.yml
- filename: constellation-brands-recipes-api-openapi.yml
  format: yaml
  label: Constellation Brands Recipes API
  slug: constellation-brands-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-recipes-api-openapi.yml
- filename: constellation-brands-shelftalkers-api-openapi.yml
  format: yaml
  label: Constellation Brands ShelfTalkers API
  slug: constellation-brands-shelftalkers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-shelftalkers-api-openapi.yml
- filename: constellation-brands-tastingnotes-api-openapi.yml
  format: yaml
  label: Constellation Brands TastingNotes API
  slug: constellation-brands-tastingnotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-tastingnotes-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Constellation Brands Authentication
name_suffix: Authentication
oauth_flows: []
overview: Constellation Brands secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Constellation Brands
provider_slug: constellation-brands
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: apiKey
  sources:
  - openapi/constellation-brands-openapi.yml
  type: apiKey
slug: constellation-brands-authentication
source_filename: constellation-brands-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/constellation-brands-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/constellation-brands-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/authentication/constellation-brands-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Alcohol
- Beer
- Beverages
- Digital Assets
- Fortune 500
- Spirits
- Wine
---
