---
api_key_in: []
api_specs:
- filename: matrix-openapi.yml
  format: yaml
  label: Matrix Client-Server API
  slug: client-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Matrix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Matrix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Matrix
provider_slug: matrix
scheme_count: 1
schemes:
- description: 'Matrix access token issued by the homeserver after login, passed as

    `Authorization: Bearer {access_token}`. Some endpoints (login,

    register, refresh) do not require authentication.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/matrix-openapi.yml
  type: http
slug: matrix-authentication
source_filename: matrix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/matrix-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Matrix access token issued by the homeserver after login, passed as\n    `Authorization: Bearer {access_token}`. Some endpoints (login,\n    register, refresh) do not require authentication.\n  sources:\n  - openapi/matrix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/authentication/matrix-authentication.yml
summary_line: http · 1 scheme
tags:
- Messaging
- Decentralized
- Federated
- Open Standard
- Real-Time Communication
- VoIP
---
