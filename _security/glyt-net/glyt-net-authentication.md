---
anonymous_access: false
api_key_in: []
api_specs:
- filename: glyt-net-receipts-api-openapi.yml
  format: yaml
  label: Glyt Receipts API
  slug: glyt-net-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glyt-net/openapi/glyt-net-receipts-api-openapi.yml
- filename: glyt-net-requests-api-openapi.yml
  format: yaml
  label: Glyt Requests API
  slug: glyt-net-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glyt-net/openapi/glyt-net-requests-api-openapi.yml
- filename: glyt-net-verify-api-openapi.yml
  format: yaml
  label: Glyt Verify API
  slug: glyt-net-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glyt-net/openapi/glyt-net-verify-api-openapi.yml
- filename: glyt-net-well-known-api-openapi.yml
  format: yaml
  label: Glyt .well Known API
  slug: glyt-net-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glyt-net/openapi/glyt-net-well-known-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Glyt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Glyt secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Glyt
provider_slug: glyt-net
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: A Colony (thecolony.cc) id_token obtained via RFC 8693 token exchange, audienced to Glyt. Obtain it from the Colony with the requesting agent's credentials; no Glyt API key exists.
  name: colonyTokenExchange
  scheme: bearer
  sources:
  - openapi/glyt-net-openapi.json
  type: http
slug: glyt-net-authentication
source_filename: glyt-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/glyt-net-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: colonyTokenExchange\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: A Colony (thecolony.cc) id_token obtained via RFC 8693 token exchange, audienced\n    to Glyt. Obtain it from the Colony with the requesting agent's credentials; no Glyt API\n    key exists.\n  sources:\n  - openapi/glyt-net-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/glyt-net/authentication/glyt-net-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Human-in-the-Loop
- Agent-Approval
- Security
- Automation
---
