---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Karaz Platform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Karaz Platform secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Karaz Platform
provider_slug: karaz-platform
scheme_count: 1
schemes:
- description: 'The Karaz API uses HTTP Bearer token authentication. Each request must carry an Authorization header using the Bearer scheme: "Authorization: Bearer {token}". Tokens are user access tokens; the docs advise keeping them secret and resetting if compromised. No OAuth2 authorization/token endpoints or scopes are documented.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.karaz.app/authentication
  type: http
slug: karaz-platform-authentication
source_filename: karaz-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.karaz.app/authentication\ndocs: https://docs.karaz.app/authentication\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    The Karaz API uses HTTP Bearer token authentication. Each request must carry\n    an Authorization header using the Bearer scheme: \"Authorization: Bearer {token}\".\n    Tokens are user access tokens; the docs advise keeping them secret and resetting\n    if compromised. No OAuth2 authorization/token endpoints or scopes are documented.\n  sources: [https://docs.karaz.app/authentication]\nnotes: >-\n  Documentation is early-stage (\"full documentation coming soon\"). No token endpoint,\n  refresh flow, or scope reference is published as of this pass.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karaz-platform/refs/heads/main/authentication/karaz-platform-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Electronic Health Records
- EHR
- Health
- Remote Patient Monitoring
- Appointments
- Artificial Intelligence
- Saudi Arabia
---
