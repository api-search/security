---
api_key_in: []
api_specs:
- filename: revcontent-access-api-openapi.yml
  format: yaml
  label: RevContent Access API
  slug: revcontent-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-access-api-openapi.yml
- filename: revcontent-boosts-api-openapi.yml
  format: yaml
  label: RevContent Boosts API
  slug: revcontent-boosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-boosts-api-openapi.yml
- filename: revcontent-ccpa-api-openapi.yml
  format: yaml
  label: RevContent CCPA API
  slug: revcontent-ccpa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-ccpa-api-openapi.yml
- filename: revcontent-content-api-openapi.yml
  format: yaml
  label: RevContent Content API
  slug: revcontent-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-content-api-openapi.yml
- filename: revcontent-helpers-api-openapi.yml
  format: yaml
  label: RevContent Helpers API
  slug: revcontent-helpers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-helpers-api-openapi.yml
- filename: revcontent-targeting-api-openapi.yml
  format: yaml
  label: RevContent Targeting API
  slug: revcontent-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-targeting-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Revcontent Authentication
name_suffix: Authentication
oauth_flows: []
overview: RevContent secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RevContent
provider_slug: revcontent
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token obtained from /oauth/token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/revcontent-stats-management-openapi.yml
  type: http
slug: revcontent-authentication
source_filename: revcontent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/revcontent-stats-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token obtained from /oauth/token\n  sources:\n  - openapi/revcontent-stats-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/authentication/revcontent-authentication.yml
summary_line: http · 1 scheme
tags:
- Native Advertising
- Content Recommendation
- Ad Network
- Publisher Monetization
- Programmatic Advertising
---
