---
anonymous_access: false
api_key_in: []
api_specs:
- filename: raute-io-drivers-api-openapi.yml
  format: yaml
  label: raute-io Drivers API
  slug: raute-io-drivers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/raute-io/openapi/raute-io-drivers-api-openapi.yml
- filename: raute-io-orders-api-openapi.yml
  format: yaml
  label: raute-io Orders API
  slug: raute-io-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/raute-io/openapi/raute-io-orders-api-openapi.yml
- filename: raute-io-tracking-api-openapi.yml
  format: yaml
  label: raute-io Tracking API
  slug: raute-io-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/raute-io/openapi/raute-io-tracking-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Raute Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: raute-io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: raute-io
provider_slug: raute-io
scheme_count: 1
schemes:
- description: 'A key created at https://www.raute.io/api-keys. The secret is shown once at creation and never again, because only its hash is stored. Each key carries scopes: tracking:read, orders:read, orders:write.'
  in: header
  name: x-api-key
  type: apiKey
slug: raute-io-authentication
source_filename: raute-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource:\n  - https://www.raute.io/openapi.json\n  - https://www.raute.io/developers/\nschemes:\n  - type: apiKey\n    in: header\n    name: x-api-key\n    description: \"A key created at https://www.raute.io/api-keys. The secret is shown once at creation and never again, because only its hash is stored. Each key carries scopes: tracking:read, orders:read, orders:write.\"\n"
source_yaml_url: https://artifacts.apis.io/raute-io/authentication/raute-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Logistics
- Delivery
- Route Planning
- AI
- Fleet Management
---
