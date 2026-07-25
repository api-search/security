---
api_key_in:
- header
api_specs:
- filename: igdb-companies-api-openapi.yml
  format: yaml
  label: IGDB Companies API
  slug: igdb-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-companies-api-openapi.yml
- filename: igdb-games-api-openapi.yml
  format: yaml
  label: IGDB Games API
  slug: igdb-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-games-api-openapi.yml
- filename: igdb-genres-api-openapi.yml
  format: yaml
  label: IGDB Genres API
  slug: igdb-genres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-genres-api-openapi.yml
- filename: igdb-media-api-openapi.yml
  format: yaml
  label: IGDB Media API
  slug: igdb-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-media-api-openapi.yml
- filename: igdb-platforms-api-openapi.yml
  format: yaml
  label: IGDB Platforms API
  slug: igdb-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-platforms-api-openapi.yml
- filename: igdb-reference-api-openapi.yml
  format: yaml
  label: IGDB Reference API
  slug: igdb-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-reference-api-openapi.yml
- filename: igdb-releases-api-openapi.yml
  format: yaml
  label: IGDB Releases API
  slug: igdb-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-releases-api-openapi.yml
- filename: igdb-search-api-openapi.yml
  format: yaml
  label: IGDB Search API
  slug: igdb-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-search-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Igdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: IGDB secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: IGDB
provider_slug: igdb
scheme_count: 2
schemes:
- description: Twitch developer Client-ID issued for the IGDB API.
  in: header
  name: ClientID
  parameter: Client-ID
  sources:
  - openapi/igdb-openapi.yml
  type: apiKey
- bearerFormat: OAuth2 access token
  description: Bearer access token obtained via the Twitch OAuth Client Credentials flow.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/igdb-openapi.yml
  type: http
slug: igdb-authentication
source_filename: igdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/igdb-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ClientID\n  type: apiKey\n  in: header\n  parameter: Client-ID\n  description: Twitch developer Client-ID issued for the IGDB API.\n  sources:\n  - openapi/igdb-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2 access token\n  description: Bearer access token obtained via the Twitch OAuth Client Credentials flow.\n  sources:\n  - openapi/igdb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/authentication/igdb-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Entertainment
- Game Database
- Gaming
- Video Games
---
