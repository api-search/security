---
api_key_in: []
api_specs:
- filename: patreon-openapi.yml
  format: yaml
  label: Patreon API v2
  slug: patreon-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patreon/refs/heads/main/openapi/patreon-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Patreon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Patreon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Patreon
provider_slug: patreon
scheme_count: 1
schemes:
- bearerFormat: OAuth2 access token
  description: 'Pass `Authorization: Bearer {access_token}`. Tokens are issued via

    the Patreon OAuth flow (`/oauth2/authorize` and `/api/oauth2/token`).'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/patreon-openapi.yml
  type: http
slug: patreon-authentication
source_filename: patreon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/patreon-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2 access token\n  description: |-\n    Pass `Authorization: Bearer {access_token}`. Tokens are issued via\n    the Patreon OAuth flow (`/oauth2/authorize` and `/api/oauth2/token`).\n  sources:\n  - openapi/patreon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patreon/refs/heads/main/authentication/patreon-authentication.yml
summary_line: http · 1 scheme
tags:
- Creator Economy
- Membership
- Subscription
- Content
- Community
---
