---
api_key_in: []
api_specs:
- filename: thundercompute-instances-api-openapi.yml
  format: yaml
  label: Thunder Compute Instances API
  slug: thundercompute-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/openapi/thundercompute-instances-api-openapi.yml
- filename: thundercompute-pricing-api-openapi.yml
  format: yaml
  label: Thunder Compute Pricing API
  slug: thundercompute-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/openapi/thundercompute-pricing-api-openapi.yml
- filename: thundercompute-snapshots-api-openapi.yml
  format: yaml
  label: Thunder Compute Snapshots API
  slug: thundercompute-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/openapi/thundercompute-snapshots-api-openapi.yml
- filename: thundercompute-specs-api-openapi.yml
  format: yaml
  label: Thunder Compute Specs API
  slug: thundercompute-specs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/openapi/thundercompute-specs-api-openapi.yml
- filename: thundercompute-ssh-keys-api-openapi.yml
  format: yaml
  label: Thunder Compute SSH Keys API
  slug: thundercompute-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/openapi/thundercompute-ssh-keys-api-openapi.yml
- filename: thundercompute-templates-api-openapi.yml
  format: yaml
  label: Thunder Compute Templates API
  slug: thundercompute-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/openapi/thundercompute-templates-api-openapi.yml
- filename: thundercompute-tokens-api-openapi.yml
  format: yaml
  label: Thunder Compute Tokens API
  slug: thundercompute-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thundercompute/refs/heads/main/openapi/thundercompute-tokens-api-openapi.yml
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
