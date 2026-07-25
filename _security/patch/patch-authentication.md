---
api_key_in: []
api_specs:
- filename: patch-order-line-items-api-openapi.yml
  format: yaml
  label: Patch Order Line Items API
  slug: patch-order-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patch/refs/heads/main/openapi/patch-order-line-items-api-openapi.yml
- filename: patch-orders-api-openapi.yml
  format: yaml
  label: Patch Orders API
  slug: patch-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patch/refs/heads/main/openapi/patch-orders-api-openapi.yml
- filename: patch-projects-api-openapi.yml
  format: yaml
  label: Patch Projects API
  slug: patch-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patch/refs/heads/main/openapi/patch-projects-api-openapi.yml
- filename: patch-technology-types-api-openapi.yml
  format: yaml
  label: Patch Technology Types API
  slug: patch-technology-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patch/refs/heads/main/openapi/patch-technology-types-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Patch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Patch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Patch
provider_slug: patch
scheme_count: 1
schemes:
- description: Bearer token API key obtained from the Patch dashboard. Use test keys for sandbox and production keys for live orders.
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/patch-patch-api-openapi.yml
  type: http
slug: patch-authentication
source_filename: patch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/patch-patch-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  description: Bearer token API key obtained from the Patch dashboard. Use test keys for sandbox\n    and production keys for live orders.\n  sources:\n  - openapi/patch-patch-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patch/refs/heads/main/authentication/patch-authentication.yml
summary_line: http · 1 scheme
tags:
- Carbon
- Carbon Credits
- Carbon Removal
- Carbon Offsets
- Sustainability
- Climate Tech
- Net Zero
- ESG
---
