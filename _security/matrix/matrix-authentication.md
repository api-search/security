---
api_key_in: []
api_specs:
- filename: matrix-account-api-openapi.yml
  format: yaml
  label: Matrix Account API
  slug: matrix-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-account-api-openapi.yml
- filename: matrix-capabilities-api-openapi.yml
  format: yaml
  label: Matrix Capabilities API
  slug: matrix-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-capabilities-api-openapi.yml
- filename: matrix-createroom-api-openapi.yml
  format: yaml
  label: Matrix CreateRoom API
  slug: matrix-createroom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-createroom-api-openapi.yml
- filename: matrix-devices-api-openapi.yml
  format: yaml
  label: Matrix Devices API
  slug: matrix-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-devices-api-openapi.yml
- filename: matrix-directory-api-openapi.yml
  format: yaml
  label: Matrix Directory API
  slug: matrix-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-directory-api-openapi.yml
- filename: matrix-join-api-openapi.yml
  format: yaml
  label: Matrix Join API
  slug: matrix-join-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-join-api-openapi.yml
- filename: matrix-keys-api-openapi.yml
  format: yaml
  label: Matrix Keys API
  slug: matrix-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-keys-api-openapi.yml
- filename: matrix-login-api-openapi.yml
  format: yaml
  label: Matrix Login API
  slug: matrix-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-login-api-openapi.yml
- filename: matrix-logout-api-openapi.yml
  format: yaml
  label: Matrix Logout API
  slug: matrix-logout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-logout-api-openapi.yml
- filename: matrix-profile-api-openapi.yml
  format: yaml
  label: Matrix Profile API
  slug: matrix-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-profile-api-openapi.yml
- filename: matrix-publicrooms-api-openapi.yml
  format: yaml
  label: Matrix PublicRooms API
  slug: matrix-publicrooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-publicrooms-api-openapi.yml
- filename: matrix-refresh-api-openapi.yml
  format: yaml
  label: Matrix Refresh API
  slug: matrix-refresh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-refresh-api-openapi.yml
- filename: matrix-register-api-openapi.yml
  format: yaml
  label: Matrix Register API
  slug: matrix-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-register-api-openapi.yml
- filename: matrix-rooms-api-openapi.yml
  format: yaml
  label: Matrix Rooms API
  slug: matrix-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-rooms-api-openapi.yml
- filename: matrix-sync-api-openapi.yml
  format: yaml
  label: Matrix Sync API
  slug: matrix-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-sync-api-openapi.yml
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
