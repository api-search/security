---
api_key_in: []
api_specs:
- filename: intralinks-authentication-api-openapi.yml
  format: yaml
  label: Intralinks Authentication API
  slug: intralinks-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-authentication-api-openapi.yml
- filename: intralinks-custom-fields-api-openapi.yml
  format: yaml
  label: Intralinks Custom Fields API
  slug: intralinks-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-custom-fields-api-openapi.yml
- filename: intralinks-documents-api-openapi.yml
  format: yaml
  label: Intralinks Documents API
  slug: intralinks-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-documents-api-openapi.yml
- filename: intralinks-folders-api-openapi.yml
  format: yaml
  label: Intralinks Folders API
  slug: intralinks-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-folders-api-openapi.yml
- filename: intralinks-groups-api-openapi.yml
  format: yaml
  label: Intralinks Groups API
  slug: intralinks-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-groups-api-openapi.yml
- filename: intralinks-permissions-api-openapi.yml
  format: yaml
  label: Intralinks Permissions API
  slug: intralinks-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-permissions-api-openapi.yml
- filename: intralinks-splash-api-openapi.yml
  format: yaml
  label: Intralinks Splash API
  slug: intralinks-splash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-splash-api-openapi.yml
- filename: intralinks-workspaces-api-openapi.yml
  format: yaml
  label: Intralinks Workspaces API
  slug: intralinks-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Intralinks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Intralinks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Intralinks
provider_slug: intralinks
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token obtained from the /oauth/token endpoint. Pass the token in the Authorization header as 'Bearer {token}'.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/intralinks-api-openapi.yml
  type: http
slug: intralinks-authentication
source_filename: intralinks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/intralinks-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token obtained from the /oauth/token endpoint. Pass the token\n    in the Authorization header as 'Bearer {token}'.\n  sources:\n  - openapi/intralinks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/authentication/intralinks-authentication.yml
summary_line: http · 1 scheme
tags:
- Document-Management
- Secure File Sharing
- Virtual Data Room
---
