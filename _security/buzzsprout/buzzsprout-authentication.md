---
api_key_in:
- header
api_specs:
- filename: buzzsprout-openapi.yml
  format: yaml
  label: Buzzsprout Episodes API
  slug: buzzsprout-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buzzsprout/refs/heads/main/openapi/buzzsprout-openapi.yml
- filename: buzzsprout-openapi.yml
  format: yaml
  label: Buzzsprout Podcasts API
  slug: buzzsprout-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buzzsprout/refs/heads/main/openapi/buzzsprout-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Buzzsprout Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buzzsprout secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Buzzsprout
provider_slug: buzzsprout
scheme_count: 1
schemes:
- description: 'Token authentication. Send the header as `Authorization: Token token=YOUR_TOKEN`. Alternatively pass the token as an `api_token` query parameter. Tokens are found in the Buzzsprout admin account settings.'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/buzzsprout-openapi.yml
  type: apiKey
slug: buzzsprout-authentication
source_filename: buzzsprout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/buzzsprout-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token authentication. Send the header as `Authorization: Token token=YOUR_TOKEN`.\n    Alternatively pass the token as an `api_token` query parameter. Tokens are found in the\n    Buzzsprout admin account settings.'\n  sources:\n  - openapi/buzzsprout-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buzzsprout/refs/heads/main/authentication/buzzsprout-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Podcasting
- Podcast Hosting
- Audio
- Media
- Episodes
- RSS
---
