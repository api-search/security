---
anonymous_access: false
api_key_in: []
api_specs:
- filename: spoken-md-balance-api-openapi.yml
  format: yaml
  label: spoken-md Balance API
  slug: spoken-md-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-balance-api-openapi.yml
- filename: spoken-md-buy-api-openapi.yml
  format: yaml
  label: spoken-md Buy API
  slug: spoken-md-buy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-buy-api-openapi.yml
- filename: spoken-md-following-api-openapi.yml
  format: yaml
  label: spoken-md Following API
  slug: spoken-md-following-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-following-api-openapi.yml
- filename: spoken-md-new-api-openapi.yml
  format: yaml
  label: spoken-md New API
  slug: spoken-md-new-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-new-api-openapi.yml
- filename: spoken-md-podcasts-api-openapi.yml
  format: yaml
  label: spoken-md Podcasts API
  slug: spoken-md-podcasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-podcasts-api-openapi.yml
- filename: spoken-md-search-api-openapi.yml
  format: yaml
  label: spoken-md Search API
  slug: spoken-md-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-search-api-openapi.yml
- filename: spoken-md-top-up-api-openapi.yml
  format: yaml
  label: spoken-md Top Up API
  slug: spoken-md-top-up-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-top-up-api-openapi.yml
- filename: spoken-md-transcripts-api-openapi.yml
  format: yaml
  label: spoken-md Transcripts API
  slug: spoken-md-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-transcripts-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Spoken Md Authentication
name_suffix: Authentication
oauth_flows: []
overview: spoken-md declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: spoken-md
provider_slug: spoken-md
scheme_count: 3
schemes:
- description: Opaque API key prefixed with pt_, sent in x-api-key header.
  in: header
  name: x-api-key
  type: apiKey
- bearerFormat: pt_ API key
  description: API key can also be sent as Bearer token in Authorization header.
  scheme: bearer
  type: http
- description: API key as username with empty password for feed readers.
  scheme: basic
  type: http
slug: spoken-md-authentication
source_filename: spoken-md-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://spoken.md/auth.md\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: Opaque API key prefixed with pt_, sent in x-api-key header.\n  - type: http\n    scheme: bearer\n    bearerFormat: pt_ API key\n    description: API key can also be sent as Bearer token in Authorization header.\n  - type: http\n    scheme: basic\n    description: API key as username with empty password for feed readers.\n"
source_yaml_url: https://artifacts.apis.io/spoken-md/authentication/spoken-md-authentication.yml
summary_line: 3 schemes
tags:
- Company
- API
- Podcast
- Transcripts
- AI
- Audio
---
