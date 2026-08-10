---
api_key_in:
- header
api_specs:
- filename: device-specs-api-values-api-openapi.yml
  format: yaml
  label: Device Specs API Values API
  slug: device-specs-api-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/device-specs-api/refs/heads/main/openapi/device-specs-api-values-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Device Specs Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Device Specs API secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Device Specs API
provider_slug: device-specs-api
scheme_count: 2
schemes:
- description: Your personal RapidAPI key.
  in: header
  name: RapidApiKey
  parameter: x-rapidapi-key
  sources:
  - openapi/device-specs-api-openapi-original.json
  type: apiKey
- description: The RapidAPI gateway host the request routes to. The spec and docs say to set it to 'deviceultraparser.p.rapidapi.com'; that host root returns HTTP 404 "API doesn't exists" while 'gsmarenaparser.p.rapidapi.com' returns a real HTTP 401 (probed 2026-08-09).
  in: header
  name: RapidApiHost
  parameter: x-rapidapi-host
  sources:
  - openapi/device-specs-api-openapi-original.json
  type: apiKey
slug: device-specs-api-authentication
source_filename: device-specs-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/device-specs-api-openapi-original.json\ndocs: https://ds.gtgroup.dev/docs\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  gateway: RapidAPI\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  applied: global\n  note: >-\n    Both schemes are required together on every operation — the spec's top-level security block lists\n    RapidApiKey and RapidApiHost in the same requirement object (AND, not OR). Credentials are issued\n    and metered by RapidAPI; there is no provider-issued credential and no self-serve key on\n    ds.gtgroup.dev.\nschemes:\n- name: RapidApiKey\n  type: apiKey\n  in: header\n  parameter: x-rapidapi-key\n  description: Your personal RapidAPI key.\n  sources:\n  - openapi/device-specs-api-openapi-original.json\n- name: RapidApiHost\n  type: apiKey\n  in: header\n  parameter: x-rapidapi-host\n  description: >-\n    The RapidAPI gateway host the request routes to. The spec\
  \ and docs say to set it to\n    'deviceultraparser.p.rapidapi.com'; that host root returns HTTP 404 \"API doesn't exists\" while\n    'gsmarenaparser.p.rapidapi.com' returns a real HTTP 401 (probed 2026-08-09).\n  sources:\n  - openapi/device-specs-api-openapi-original.json\nkey_issuance:\n  url: https://rapidapi.com/controller2042000/api/gsmarenaparser\n  self_serve: true\n  free_tier: true\n  note: A RapidAPI account and a subscription (BASIC is $0) are required before any call succeeds.\nscopes:\n  supported: false\n  note: No OAuth, no scope model, no per-key permissioning documented. Access is all-or-nothing per subscription tier.\nrotation:\n  documented: false\ntransport:\n  https_required: true\n  tls_version_observed: TLSv1.2\n  observed_host: gsmarenaparser.p.rapidapi.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/device-specs-api/refs/heads/main/authentication/device-specs-api-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- mobile
- smartphones
- phone-specs
- chipsets
- hardware
- mobile-specs
- devices
- rapidapi
- gsmarena
- reference-data
- developer-tools
---
