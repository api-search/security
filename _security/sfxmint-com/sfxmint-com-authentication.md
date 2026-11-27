---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sfxmint-com-generation-api-openapi.yml
  format: yaml
  label: SFXMint Generation API
  slug: sfxmint-com-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sfxmint-com/openapi/sfxmint-com-generation-api-openapi.yml
- filename: sfxmint-com-library-api-openapi.yml
  format: yaml
  label: SFXMint Library API
  slug: sfxmint-com-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sfxmint-com/openapi/sfxmint-com-library-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: SFXMint Authentication
name_suffix: Authentication
oauth_flows: []
overview: SFXMint secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SFXMint
provider_slug: sfxmint-com
scheme_count: 1
schemes:
- description: An SFXMint API key (sfx_live_…). X-API-Key is accepted too.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/sfxmint-com-openapi.yml
  type: http
slug: sfxmint-com-authentication
source_filename: sfxmint-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/sfxmint-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: An SFXMint API key (sfx_live_…). X-API-Key is accepted too.\n  sources:\n  - openapi/sfxmint-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/sfxmint-com/authentication/sfxmint-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Sound Effects
- CC0
- AI Studio
- Games
- Free
---
