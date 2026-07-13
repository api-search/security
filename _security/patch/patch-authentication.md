---
api_key_in: []
api_specs:
- filename: index.html
  format: yaml
  label: Patch API
  slug: patch-api
  spec_type: OpenAPI
  url: https://api.patch.io/api-docs/index.html
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
