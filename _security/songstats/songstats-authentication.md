---
api_key_in:
- header
api_specs:
- filename: songstats-artists-api-openapi.yml
  format: yaml
  label: Songstats Artists API
  slug: songstats-artists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songstats/refs/heads/main/openapi/songstats-artists-api-openapi.yml
- filename: songstats-collaborators-api-openapi.yml
  format: yaml
  label: Songstats Collaborators API
  slug: songstats-collaborators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songstats/refs/heads/main/openapi/songstats-collaborators-api-openapi.yml
- filename: songstats-info-api-openapi.yml
  format: yaml
  label: Songstats Info API
  slug: songstats-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songstats/refs/heads/main/openapi/songstats-info-api-openapi.yml
- filename: songstats-labels-api-openapi.yml
  format: yaml
  label: Songstats Labels API
  slug: songstats-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songstats/refs/heads/main/openapi/songstats-labels-api-openapi.yml
- filename: songstats-tracks-api-openapi.yml
  format: yaml
  label: Songstats Tracks API
  slug: songstats-tracks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songstats/refs/heads/main/openapi/songstats-tracks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Songstats Authentication
name_suffix: Authentication
oauth_flows: []
overview: Songstats secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Songstats
provider_slug: songstats
scheme_count: 1
schemes:
- description: API key from the Songstats Enterprise dashboard. Contact api@songstats.com for access.
  in: header
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/songstats-openapi.yml
  type: apiKey
slug: songstats-authentication
source_filename: songstats-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/songstats-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: API key from the Songstats Enterprise dashboard. Contact api@songstats.com for\n    access.\n  sources:\n  - openapi/songstats-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/songstats/refs/heads/main/authentication/songstats-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Music
- Streaming
- Artists
- Tracks
- Labels
---
