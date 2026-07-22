---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Turneo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Turneo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Turneo
provider_slug: turneo
scheme_count: 1
schemes:
- description: Every request to the Turneo v2 API must include a partner API key in the X-API-Key request header. Keys are issued per partner/store from the Turneo dashboard (app.turneo.co). No OAuth or OpenID Connect flow is documented; the API key is the sole credential.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - docs:getting-started
  type: apiKey
slug: turneo-authentication
source_filename: turneo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.turneo.com/developers/guides/getting-started\ndocs: https://www.turneo.com/developers/guides/getting-started\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    description: >-\n      Every request to the Turneo v2 API must include a partner API key in the\n      X-API-Key request header. Keys are issued per partner/store from the\n      Turneo dashboard (app.turneo.co). No OAuth or OpenID Connect flow is\n      documented; the API key is the sole credential.\n    sources: [docs:getting-started]\nnotes: >-\n  API host https://api.turneo.co returns HTTP 401 for all unauthenticated\n  requests (edge-gated), so no public OpenAPI/Swagger document is available to\n  derive from. This profile is captured from the published developer guides.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turneo/refs/heads/main/authentication/turneo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Marketplaces
- Travel
- Hospitality
- Hotels
- Experiences
- Booking
- Activities
- Tours
---
