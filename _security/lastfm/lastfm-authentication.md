---
api_key_in:
- query
api_specs:
- filename: lastfm-openapi-original.yml
  format: yaml
  label: Last.fm Web Services 2.0
  slug: lastfm-web-services-2-0
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lastfm/refs/heads/main/openapi/lastfm-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lastfm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Last.fm secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Last.fm
provider_slug: lastfm
scheme_count: 2
schemes:
- description: Required on all calls. Obtain from https://www.last.fm/api/account/create.
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/lastfm-openapi-original.yml
  type: apiKey
- description: 'MD5 signature of all request parameters (excluding format and callback)

    sorted alphabetically by name, concatenated as name+value pairs, with

    the shared secret appended. Required for all write/auth methods.'
  in: query
  name: SignedAuth
  parameter: api_sig
  sources:
  - openapi/lastfm-openapi-original.yml
  type: apiKey
slug: lastfm-authentication
source_filename: lastfm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lastfm-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Required on all calls. Obtain from https://www.last.fm/api/account/create.\n  sources:\n  - openapi/lastfm-openapi-original.yml\n- name: SignedAuth\n  type: apiKey\n  in: query\n  parameter: api_sig\n  description: |-\n    MD5 signature of all request parameters (excluding format and callback)\n    sorted alphabetically by name, concatenated as name+value pairs, with\n    the shared secret appended. Required for all write/auth methods.\n  sources:\n  - openapi/lastfm-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lastfm/refs/heads/main/authentication/lastfm-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Music
- Audio
- Scrobbling
- Recommendations
- Charts
- Public APIs
- AudioScrobbler
---
