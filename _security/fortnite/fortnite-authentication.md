---
api_key_in:
- header
api_specs:
- filename: fortnite-tracker.yaml
  format: yaml
  label: Fortnite Tracker
  slug: fortnite-tracker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnite/refs/heads/main/openapi/fortnite-tracker.yaml
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
