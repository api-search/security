---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: agilis-dating-events-api-openapi.yml
  format: yaml
  label: Agilis Dating Ltd Events API
  slug: agilis-dating-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilis-dating/openapi/agilis-dating-events-api-openapi.yml
- filename: agilis-dating-offers-api-openapi.yml
  format: yaml
  label: Agilis Dating Ltd Offers API
  slug: agilis-dating-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilis-dating/openapi/agilis-dating-offers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agilis Dating Ltd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agilis Dating Ltd secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agilis Dating Ltd
provider_slug: agilis-dating
scheme_count: 1
schemes:
- description: Created in the Ad Portal under Manage API Keys. Shown once; Roll key replaces a lost one. One key per mode (TEST or LIVE).
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/agilis-dating-openapi.json
  type: apiKey
slug: agilis-dating-authentication
source_filename: agilis-dating-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/agilis-dating-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Created in the Ad Portal under Manage API Keys. Shown once; Roll key replaces\n    a lost one. One key per mode (TEST or LIVE).\n  sources:\n  - openapi/agilis-dating-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/agilis-dating/authentication/agilis-dating-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Dating
- Advertising
- Free
- United Kingdom
---
