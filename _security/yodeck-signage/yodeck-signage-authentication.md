---
api_key_in:
- header
api_specs:
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Media API
  slug: yodeck-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Playlists API
  slug: yodeck-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Layouts API
  slug: yodeck-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Screens API
  slug: yodeck-screens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Schedules API
  slug: yodeck-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Shows API
  slug: yodeck-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
- filename: yodeck-signage-openapi.yml
  format: yaml
  label: Yodeck Workspaces API
  slug: yodeck-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/openapi/yodeck-signage-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Yodeck Signage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yodeck secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Yodeck
provider_slug: yodeck-signage
scheme_count: 1
schemes:
- description: Named, role-scoped API token generated in the Yodeck console (Account Settings > Advanced Settings > API Tokens). The token acts as a user with the permissions of its assigned role. Send it in the Authorization header. The exact header value format (for example "Token name:secret") is documented in the login-gated reference and should be confirmed there.
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/yodeck-signage-openapi.yml
  type: apiKey
slug: yodeck-signage-authentication
source_filename: yodeck-signage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/yodeck-signage-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Named, role-scoped API token generated in the Yodeck console (Account Settings\n    > Advanced Settings > API Tokens). The token acts as a user with the permissions of its\n    assigned role. Send it in the Authorization header. The exact header value format (for example\n    \"Token name:secret\") is documented in the login-gated reference and should be confirmed\n    there.\n  sources:\n  - openapi/yodeck-signage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yodeck-signage/refs/heads/main/authentication/yodeck-signage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Digital Signage
- Screen Management
- Content Management
- Media
- Playlists
- Scheduling
- Raspberry Pi
---
