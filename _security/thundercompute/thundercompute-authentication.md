---
api_key_in: []
api_specs:
- filename: thundercompute-openapi.yml
  format: yaml
  label: Thunder Compute Instances API
  slug: thundercompute-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/openapi/thundercompute-openapi.yml
- filename: thundercompute-openapi.yml
  format: yaml
  label: Thunder Compute Snapshots API
  slug: thundercompute-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/openapi/thundercompute-openapi.yml
- filename: thundercompute-openapi.yml
  format: yaml
  label: Thunder Compute Account API
  slug: thundercompute-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/openapi/thundercompute-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Thundercompute Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thunder Compute secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Thunder Compute
provider_slug: thundercompute
scheme_count: 1
schemes:
- description: API token generated in the Thunder Compute console (console.thundercompute.com/settings/tokens), sent as a Bearer token in the Authorization header. The tnr CLI reads it from the TNR_API_TOKEN environment variable.
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/thundercompute-openapi.yml
  type: http
slug: thundercompute-authentication
source_filename: thundercompute-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thundercompute-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: API token generated in the Thunder Compute console (console.thundercompute.com/settings/tokens),\n    sent as a Bearer token in the Authorization header. The tnr CLI reads it from the TNR_API_TOKEN\n    environment variable.\n  sources:\n  - openapi/thundercompute-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/authentication/thundercompute-authentication.yml
summary_line: http · 1 scheme
tags:
- GPU
- Cloud
- Infrastructure
- AI
- Compute
---
