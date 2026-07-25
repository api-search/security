---
api_key_in:
- query
api_specs:
- filename: giphy-analytics-api-openapi.yml
  format: yaml
  label: Giphy Analytics API
  slug: giphy-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/openapi/giphy-analytics-api-openapi.yml
- filename: giphy-animate-api-openapi.yml
  format: yaml
  label: Giphy Animate API
  slug: giphy-animate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/openapi/giphy-animate-api-openapi.yml
- filename: giphy-categories-api-openapi.yml
  format: yaml
  label: Giphy Categories API
  slug: giphy-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/openapi/giphy-categories-api-openapi.yml
- filename: giphy-channels-api-openapi.yml
  format: yaml
  label: Giphy Channels API
  slug: giphy-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/openapi/giphy-channels-api-openapi.yml
- filename: giphy-clips-api-openapi.yml
  format: yaml
  label: Giphy Clips API
  slug: giphy-clips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/openapi/giphy-clips-api-openapi.yml
- filename: giphy-emoji-api-openapi.yml
  format: yaml
  label: Giphy Emoji API
  slug: giphy-emoji-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/openapi/giphy-emoji-api-openapi.yml
- filename: giphy-gifs-api-openapi.yml
  format: yaml
  label: Giphy GIFs API
  slug: giphy-gifs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/openapi/giphy-gifs-api-openapi.yml
- filename: giphy-search-discovery-api-openapi.yml
  format: yaml
  label: Giphy Search Discovery API
  slug: giphy-search-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/openapi/giphy-search-discovery-api-openapi.yml
- filename: giphy-stickers-api-openapi.yml
  format: yaml
  label: Giphy Stickers API
  slug: giphy-stickers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/openapi/giphy-stickers-api-openapi.yml
- filename: giphy-upload-api-openapi.yml
  format: yaml
  label: Giphy Upload API
  slug: giphy-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/openapi/giphy-upload-api-openapi.yml
- filename: giphy-utilities-api-openapi.yml
  format: yaml
  label: Giphy Utilities API
  slug: giphy-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/openapi/giphy-utilities-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Giphy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Giphy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Giphy
provider_slug: giphy
scheme_count: 1
schemes:
- description: API key issued via the GIPHY developer dashboard.
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/giphy-openapi.yml
  type: apiKey
slug: giphy-authentication
source_filename: giphy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/giphy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key issued via the GIPHY developer dashboard.\n  sources:\n  - openapi/giphy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/authentication/giphy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Photography
- Media
- GIFs
- Stickers
- Emoji
- Video
- Messaging
- Social
- Meta
---
