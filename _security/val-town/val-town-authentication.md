---
api_key_in: []
api_specs:
- filename: val-town-alias-api-openapi.yml
  format: yaml
  label: Val Town alias API
  slug: val-town-alias-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/openapi/val-town-alias-api-openapi.yml
- filename: val-town-blobs-api-openapi.yml
  format: yaml
  label: Val Town blobs API
  slug: val-town-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/openapi/val-town-blobs-api-openapi.yml
- filename: val-town-connections-api-openapi.yml
  format: yaml
  label: Val Town connections API
  slug: val-town-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/openapi/val-town-connections-api-openapi.yml
- filename: val-town-emails-api-openapi.yml
  format: yaml
  label: Val Town emails API
  slug: val-town-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/openapi/val-town-emails-api-openapi.yml
- filename: val-town-files-api-openapi.yml
  format: yaml
  label: Val Town files API
  slug: val-town-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/openapi/val-town-files-api-openapi.yml
- filename: val-town-me-api-openapi.yml
  format: yaml
  label: Val Town me API
  slug: val-town-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/openapi/val-town-me-api-openapi.yml
- filename: val-town-orgs-api-openapi.yml
  format: yaml
  label: Val Town orgs API
  slug: val-town-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/openapi/val-town-orgs-api-openapi.yml
- filename: val-town-sqlite-api-openapi.yml
  format: yaml
  label: Val Town sqlite API
  slug: val-town-sqlite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/openapi/val-town-sqlite-api-openapi.yml
- filename: val-town-telemetry-api-openapi.yml
  format: yaml
  label: Val Town telemetry API
  slug: val-town-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/openapi/val-town-telemetry-api-openapi.yml
- filename: val-town-users-api-openapi.yml
  format: yaml
  label: Val Town users API
  slug: val-town-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/openapi/val-town-users-api-openapi.yml
- filename: val-town-vals-api-openapi.yml
  format: yaml
  label: Val Town vals API
  slug: val-town-vals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/openapi/val-town-vals-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Val Town Authentication
name_suffix: Authentication
oauth_flows: []
overview: Val Town secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Val Town
provider_slug: val-town
scheme_count: 1
schemes:
- description: Endpoints that support authorization expect Bearer authentication, using an API token provided from Val Town.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/val-town-rest-api-openapi.yml
  type: http
slug: val-town-authentication
source_filename: val-town-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/val-town-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Endpoints that support authorization expect Bearer authentication, using an API\n    token provided from Val Town.\n  sources:\n  - openapi/val-town-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/val-town/refs/heads/main/authentication/val-town-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer Tools
- Serverless
- JavaScript
- TypeScript
- Social Coding
- HTTP Endpoints
- Cron Jobs
- Email
- SQLite
- Blob Storage
---
