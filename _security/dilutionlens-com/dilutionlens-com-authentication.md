---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dilutionlens-com-company-api-openapi.yml
  format: yaml
  label: DilutionLens Company API
  slug: dilutionlens-com-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dilutionlens-com/openapi/dilutionlens-com-company-api-openapi.yml
- filename: dilutionlens-com-screen-api-openapi.yml
  format: yaml
  label: DilutionLens Screen API
  slug: dilutionlens-com-screen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dilutionlens-com/openapi/dilutionlens-com-screen-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dilutionlens Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DilutionLens secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DilutionLens
provider_slug: dilutionlens-com
scheme_count: 1
schemes:
- description: Created and revoked at https://dilutionlens.com/account/. Shown once at creation; stored hashed.
  in: header
  name: apiKey
  notes:
  - Send your key as the x-api-key header — not Authorization, which our CDN reserves.
  - A key is shown once at creation and stored hashed; revocation takes effect immediately.
  - Snapshot and options endpoints and the get_dilution_snapshot MCP tool work with no key; paid tools follow your plan.
  parameter: x-api-key
  sources:
  - openapi/dilutionlens-com-openapi.yml
  type: apiKey
slug: dilutionlens-com-authentication
source_filename: dilutionlens-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://dilutionlens.com/developers/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Created and revoked at https://dilutionlens.com/account/. Shown once\n    at creation; stored hashed.\n  sources:\n  - openapi/dilutionlens-com-openapi.yml\n  notes:\n  - Send your key as the x-api-key header — not Authorization, which our CDN reserves.\n  - A key is shown once at creation and stored hashed; revocation takes effect immediately.\n  - Snapshot and options endpoints and the get_dilution_snapshot MCP tool work with\n    no key; paid tools follow your plan.\ndocs: https://dilutionlens.com/developers/\nkey_prefix: dlk_\n"
source_yaml_url: https://artifacts.apis.io/dilutionlens-com/authentication/dilutionlens-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Financial Data
- Capital Markets
- ASX
- Equity Dilution
- Market Data
- MCP
- Investing
---
