---
api_key_in:
- header
api_specs:
- filename: magic-link-openapi.yml
  format: yaml
  label: Magic Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-link/refs/heads/main/openapi/magic-link-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Magic Link Authentication
name_suffix: Authentication
oauth_flows: []
overview: Magic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Magic
provider_slug: magic-link
scheme_count: 1
schemes:
- description: Workspace secret API key from the Magic dashboard.
  in: header
  name: SecretKey
  parameter: X-Magic-Secret-Key
  sources:
  - openapi/magic-link-openapi.yml
  type: apiKey
slug: magic-link-authentication
source_filename: magic-link-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/magic-link-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SecretKey\n  type: apiKey\n  in: header\n  parameter: X-Magic-Secret-Key\n  description: Workspace secret API key from the Magic dashboard.\n  sources:\n  - openapi/magic-link-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magic-link/refs/heads/main/authentication/magic-link-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Wallets
- Authentication
- Embedded Wallets
- MPC
---
