---
api_key_in:
- header
api_specs:
- filename: toornament-openapi.yml
  format: yaml
  label: Toornament Organizer API
  slug: organizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Toornament Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Toornament secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Toornament
provider_slug: toornament
scheme_count: 2
schemes:
- description: API key obtained from the Toornament developer dashboard.
  in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/toornament-openapi.yml
  type: apiKey
- description: OAuth2 access token with scoped permissions (organizer:view, organizer:admin).
  flows:
  - authorizationUrl: https://app.toornament.com/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api.toornament.com/oauth/v2/token
  name: oauth2
  sources:
  - openapi/toornament-openapi.yml
  type: oauth2
slug: toornament-authentication
source_filename: toornament-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/toornament-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key obtained from the Toornament developer dashboard.\n  sources:\n  - openapi/toornament-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.toornament.com/oauth/authorize\n    tokenUrl: https://api.toornament.com/oauth/v2/token\n    scopes: 3\n  description: OAuth2 access token with scoped permissions (organizer:view, organizer:admin).\n  sources:\n  - openapi/toornament-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/authentication/toornament-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Esports
- Gaming
- Tournaments
- Brackets
- Competition
---
