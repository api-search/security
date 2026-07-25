---
api_key_in:
- header
api_specs:
- filename: fortnite-challenges-api-openapi.yml
  format: yaml
  label: Fortnite Tracker Challenges API
  slug: fortnite-challenges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnite/refs/heads/main/openapi/fortnite-challenges-api-openapi.yml
- filename: fortnite-leaderboards-api-openapi.yml
  format: yaml
  label: Fortnite Tracker Leaderboards API
  slug: fortnite-leaderboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnite/refs/heads/main/openapi/fortnite-leaderboards-api-openapi.yml
- filename: fortnite-power-rankings-api-openapi.yml
  format: yaml
  label: Fortnite Tracker Power Rankings API
  slug: fortnite-power-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnite/refs/heads/main/openapi/fortnite-power-rankings-api-openapi.yml
- filename: fortnite-profile-api-openapi.yml
  format: yaml
  label: Fortnite Tracker Profile API
  slug: fortnite-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnite/refs/heads/main/openapi/fortnite-profile-api-openapi.yml
- filename: fortnite-store-api-openapi.yml
  format: yaml
  label: Fortnite Tracker Store API
  slug: fortnite-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnite/refs/heads/main/openapi/fortnite-store-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fortnite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fortnite Tracker secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fortnite Tracker
provider_slug: fortnite
scheme_count: 1
schemes:
- description: Per-account API key issued from https://fortnitetracker.com/site-api/create. Pass as the `TRN-Api-Key` request header. Default rate limit is approximately one request per two seconds per key.
  in: header
  name: trnApiKey
  parameter: TRN-Api-Key
  sources:
  - openapi/fortnite-tracker.yaml
  type: apiKey
slug: fortnite-authentication
source_filename: fortnite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fortnite-tracker.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: trnApiKey\n  type: apiKey\n  in: header\n  parameter: TRN-Api-Key\n  description: Per-account API key issued from https://fortnitetracker.com/site-api/create.\n    Pass as the `TRN-Api-Key` request header. Default rate limit is approximately one request\n    per two seconds per key.\n  sources:\n  - openapi/fortnite-tracker.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortnite/refs/heads/main/authentication/fortnite-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Games And Comics
- Public APIs
- Fortnite
- Player Statistics
- Esports
- Tracker Network
---
