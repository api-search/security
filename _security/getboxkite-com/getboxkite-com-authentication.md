---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getboxkite-com-exports-api-openapi.yml
  format: yaml
  label: Boxkite Exports API
  slug: getboxkite-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getboxkite-com/openapi/getboxkite-com-exports-api-openapi.yml
- filename: getboxkite-com-organisations-api-openapi.yml
  format: yaml
  label: Boxkite Organisations API
  slug: getboxkite-com-organisations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getboxkite-com/openapi/getboxkite-com-organisations-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Boxkite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boxkite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Boxkite
provider_slug: getboxkite-com
scheme_count: 1
schemes:
- description: Boxkite API key created at https://app.getboxkite.com/settings/api-keys (sign in first; shown once), sent as a bearer token. OAuth 2.1 access tokens are also accepted for the MCP server.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/getboxkite-com-openapi.yml
  type: http
slug: getboxkite-com-authentication
source_filename: getboxkite-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/getboxkite-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Boxkite API key created at https://app.getboxkite.com/settings/api-keys (sign\n    in first; shown once), sent as a bearer token. OAuth 2.1 access tokens are also accepted\n    for the MCP server.\n  sources:\n  - openapi/getboxkite-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/getboxkite-com/authentication/getboxkite-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Accounting
- Backup
- Cloud Storage
- New Zealand
- Small Business
---
