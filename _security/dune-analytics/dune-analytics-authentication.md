---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dune Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dune Analytics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dune Analytics
provider_slug: dune-analytics
scheme_count: 1
schemes:
- in: header
  name: DuneApiKey
  parameter: X-Dune-API-Key
  sources:
  - openapi/dune-analytics-openapi.yml
  type: apiKey
slug: dune-analytics-authentication
source_filename: dune-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dune-analytics-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: DuneApiKey\n  type: apiKey\n  in: header\n  parameter: X-Dune-API-Key\n  sources:\n  - openapi/dune-analytics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dune-analytics/refs/heads/main/authentication/dune-analytics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Analytics
- SQL
- Dashboards
- Blockchain
- Onchain
- Multi-chain
---
