---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: freqblog-com-audio-api-openapi.yml
  format: yaml
  label: freqblog-com Audio API
  slug: freqblog-com-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freqblog-com/openapi/freqblog-com-audio-api-openapi.yml
- filename: freqblog-com-backfill-api-openapi.yml
  format: yaml
  label: freqblog-com Backfill API
  slug: freqblog-com-backfill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freqblog-com/openapi/freqblog-com-backfill-api-openapi.yml
- filename: freqblog-com-catalog-api-openapi.yml
  format: yaml
  label: freqblog-com Catalog API
  slug: freqblog-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freqblog-com/openapi/freqblog-com-catalog-api-openapi.yml
- filename: freqblog-com-me-api-openapi.yml
  format: yaml
  label: freqblog-com Me API
  slug: freqblog-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freqblog-com/openapi/freqblog-com-me-api-openapi.yml
- filename: freqblog-com-request-free-key-api-openapi.yml
  format: yaml
  label: freqblog-com Request Free Key API
  slug: freqblog-com-request-free-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freqblog-com/openapi/freqblog-com-request-free-key-api-openapi.yml
- filename: freqblog-com-spotify-compat-api-openapi.yml
  format: yaml
  label: freqblog-com Spotify Compat API
  slug: freqblog-com-spotify-compat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freqblog-com/openapi/freqblog-com-spotify-compat-api-openapi.yml
- filename: freqblog-com-system-api-openapi.yml
  format: yaml
  label: freqblog-com System API
  slug: freqblog-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freqblog-com/openapi/freqblog-com-system-api-openapi.yml
- filename: freqblog-com-utility-api-openapi.yml
  format: yaml
  label: freqblog-com Utility API
  slug: freqblog-com-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freqblog-com/openapi/freqblog-com-utility-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Freqblog Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: freqblog-com secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: freqblog-com
provider_slug: freqblog-com
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/freqblog-com-openapi.json
  - openapi/freqblog-com-openapi1.json
  type: apiKey
slug: freqblog-com-authentication
source_filename: freqblog-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/freqblog-com-openapi.json, openapi/freqblog-com-openapi1.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/freqblog-com-openapi.json\n  - openapi/freqblog-com-openapi1.json\n"
source_yaml_url: https://artifacts.apis.io/freqblog-com/authentication/freqblog-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Music
- API
- Audio
- Metadata
---
