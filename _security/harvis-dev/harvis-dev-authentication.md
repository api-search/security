---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: harvis-dev-files-api-openapi.yml
  format: yaml
  label: Harvis Files API
  slug: harvis-dev-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harvis-dev/openapi/harvis-dev-files-api-openapi.yml
- filename: harvis-dev-keys-api-openapi.yml
  format: yaml
  label: Harvis Keys API
  slug: harvis-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harvis-dev/openapi/harvis-dev-keys-api-openapi.yml
- filename: harvis-dev-meta-api-openapi.yml
  format: yaml
  label: Harvis Meta API
  slug: harvis-dev-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harvis-dev/openapi/harvis-dev-meta-api-openapi.yml
- filename: harvis-dev-sites-api-openapi.yml
  format: yaml
  label: Harvis Sites API
  slug: harvis-dev-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harvis-dev/openapi/harvis-dev-sites-api-openapi.yml
- filename: harvis-dev-submissions-api-openapi.yml
  format: yaml
  label: Harvis Submissions API
  slug: harvis-dev-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harvis-dev/openapi/harvis-dev-submissions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Harvis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harvis secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Harvis
provider_slug: harvis-dev
scheme_count: 2
schemes:
- bearerFormat: hvs_…
  description: An account key, created at https://harvis.dev/dashboard/keys and shown once.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/harvis-dev-openapi.json
  type: http
- description: The dashboard's own sign-in cookie. Listed because the browser calls these same endpoints; a CLI or a server should use apiKey instead.
  in: cookie
  name: session
  parameter: better-auth.session_token
  sources:
  - openapi/harvis-dev-openapi.json
  type: apiKey
slug: harvis-dev-authentication
source_filename: harvis-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/harvis-dev-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: hvs_…\n  description: An account key, created at https://harvis.dev/dashboard/keys and shown once.\n  sources:\n  - openapi/harvis-dev-openapi.json\n- name: session\n  type: apiKey\n  in: cookie\n  parameter: better-auth.session_token\n  description: The dashboard's own sign-in cookie. Listed because the browser calls these same\n    endpoints; a CLI or a server should use apiKey instead.\n  sources:\n  - openapi/harvis-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/harvis-dev/authentication/harvis-dev-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Deployment
- Static Sites
- Developer Tools
---
