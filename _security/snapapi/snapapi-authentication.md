---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: SnapAPI
  slug: snapapi
  spec_type: OpenAPI
  url: https://snap.michaelcli.com/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Snapapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: SnapAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SnapAPI
provider_slug: snapapi
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/snapapi-openapi.json
  type: apiKey
slug: snapapi-authentication
source_filename: snapapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snapapi-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/snapapi-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapapi/refs/heads/main/authentication/snapapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Screenshots
- Website Screenshots
- Metadata Extraction
- Text Extraction
- PDF Generation
- Headless Chromium
- Web Scraping
- Developer Tools
- REST
---
