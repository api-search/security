---
api_key_in:
- header
api_specs:
- filename: one-codex-openapi-original.json
  format: json
  label: One Codex API (v1)
  slug: one-codex-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-codex/refs/heads/main/openapi/one-codex-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: One Codex Authentication
name_suffix: Authentication
oauth_flows: []
overview: One Codex secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: One Codex
provider_slug: one-codex
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/one-codex-openapi-original.json
  type: apiKey
slug: one-codex-authentication
source_filename: one-codex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/one-codex-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/one-codex-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-codex/refs/heads/main/authentication/one-codex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Genomics
- Microbiome
- Bioinformatics
- Metagenomics
- Life Sciences
- Sequencing
- Healthcare
- Data Platform
- API
---
