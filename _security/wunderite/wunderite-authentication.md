---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Wunderite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wunderite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wunderite
provider_slug: wunderite
scheme_count: 1
schemes:
- description: 'API key passed as a bearer token — "Authorization: Bearer {token}" with "Accept: application/json". Keys are generated in Wunderite under Account > Settings > Integrations; docs recommend creating a dedicated API User for programmatic access.'
  name: bearerAuth
  scheme: bearer
  type: http
slug: wunderite-authentication
source_filename: wunderite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.wunderite.com/quickstart\ndocs: https://docs.wunderite.com/quickstart\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API key passed as a bearer token — \"Authorization: Bearer {token}\" with\n    \"Accept: application/json\". Keys are generated in Wunderite under\n    Account > Settings > Integrations; docs recommend creating a dedicated\n    API User for programmatic access.\nnotes:\n- No OAuth 2.0 or OpenID Connect surface documented.\n- No public OpenAPI spec published; profile captured from the docs quickstart.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wunderite/refs/heads/main/authentication/wunderite-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Insurance
- Insurtech
- ACORD Forms
- Risk Data
- Digital Signatures
- Insurance Applications
- Webhooks
---
