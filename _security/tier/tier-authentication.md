---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tier secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tier
provider_slug: tier
scheme_count: 1
schemes:
- description: Partner API Key obtained via Dott's registration process, sent as an authorization header on requests to the Dott Partner API / GBFS host.
  in: header
  name: apiKey
  sources:
  - https://ridedott.com/api-licence/
  type: apiKey
slug: tier-authentication
source_filename: tier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://ridedott.com/api-licence/\ndocs: https://ridedott.com/api-licence/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    The Dott Partner API is gated by a per-partner API Key issued through a\n    registration process communicated by Dott (see the published API Licence).\n    Keys are non-transferable (\"You may not share the API Key with any third\n    party\"). No public OpenAPI or OAuth surface is published; the GBFS data host\n    (gbfs.api.ridedott.com) rejects unauthenticated requests with HTTP 401\n    (\"Unauthorized: missing authorization header\").\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    description: >-\n      Partner API Key obtained via Dott's registration process, sent as an\n      authorization header on requests to the Dott Partner API / GBFS host.\n    sources: [https://ridedott.com/api-licence/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tier/refs/heads/main/authentication/tier-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Micromobility
- Transportation
- Mobility
- Scooters
- E-Bikes
- GBFS
- Europe
---
