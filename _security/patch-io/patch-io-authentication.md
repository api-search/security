---
api_key_in: []
api_specs:
- filename: patch-io-order-line-items-api-openapi.yml
  format: yaml
  label: Patch Order Line Items API
  slug: patch-io-order-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patch-io/refs/heads/main/openapi/patch-io-order-line-items-api-openapi.yml
- filename: patch-io-orders-api-openapi.yml
  format: yaml
  label: Patch Orders API
  slug: patch-io-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patch-io/refs/heads/main/openapi/patch-io-orders-api-openapi.yml
- filename: patch-io-projects-api-openapi.yml
  format: yaml
  label: Patch Projects API
  slug: patch-io-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patch-io/refs/heads/main/openapi/patch-io-projects-api-openapi.yml
- filename: patch-io-technology-types-api-openapi.yml
  format: yaml
  label: Patch Technology Types API
  slug: patch-io-technology-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patch-io/refs/heads/main/openapi/patch-io-technology-types-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Patch Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Patch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Patch
provider_slug: patch-io
scheme_count: 1
schemes:
- description: API key bearer token issued from the Patch dashboard. Sandbox and live keys are separated.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/patch-io-carbon-api-openapi.yml
  type: http
slug: patch-io-authentication
source_filename: patch-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/patch-io-carbon-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key bearer token issued from the Patch dashboard. Sandbox and live keys are\n    separated.\n  sources:\n  - openapi/patch-io-carbon-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patch-io/refs/heads/main/authentication/patch-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Climate
- Carbon Credits
- Carbon Removal
- Offsets
- API-First
- Embedded Climate
- Marketplace
- Sustainability
- OpenAPI
- SDK
---
