---
api_key_in:
- query
api_specs:
- filename: last-fm-openapi.yml
  format: yaml
  label: Last.fm API
  slug: last-fm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/last-fm/refs/heads/main/openapi/last-fm-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Last Fm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Last.fm secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Last.fm
provider_slug: last-fm
scheme_count: 2
schemes:
- description: A Last.fm API key obtained from https://www.last.fm/api/account/create
  in: query
  name: ApiKey
  parameter: api_key
  sources:
  - openapi/last-fm-openapi.yml
  type: apiKey
- description: A session key obtained via the Last.fm authentication flow (auth.getSession or auth.getMobileSession)
  in: query
  name: SessionKey
  parameter: sk
  sources:
  - openapi/last-fm-openapi.yml
  type: apiKey
slug: last-fm-authentication
source_filename: last-fm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/last-fm-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: A Last.fm API key obtained from https://www.last.fm/api/account/create\n  sources:\n  - openapi/last-fm-openapi.yml\n- name: SessionKey\n  type: apiKey\n  in: query\n  parameter: sk\n  description: A session key obtained via the Last.fm authentication flow (auth.getSession or\n    auth.getMobileSession)\n  sources:\n  - openapi/last-fm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/last-fm/refs/heads/main/authentication/last-fm-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Music
- Music Metadata
- Scrobbling
- Music Discovery
- Streaming
---
