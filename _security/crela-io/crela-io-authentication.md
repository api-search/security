---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crela-io-openapi-generated.yml
  format: yaml
  label: Crela API
  slug: crela-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crela-io/openapi/_ae-authored/crela-io-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Crela Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crela declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Crela
provider_slug: crela-io
scheme_count: 1
schemes:
- description: All endpoints except GET /api/agent/requirements require a Bearer token. Keys are created in the creator dashboard (https://crela.io/dashboard/creator/keys); the full key is shown once on creation. No limit on active keys.
  env_var: CRELA_API_KEY
  format: 'Authorization: Bearer crela_<your-api-key>'
  header: Authorization
  key_management:
  - POST /api/agent/keys (create; returns the full key once)
  - PATCH /api/agent/keys/{id} (rename)
  - DELETE /api/agent/keys/{id} (revoke; takes effect immediately)
  key_prefix: crela_
  name: Crela API key
  scheme: bearer
  type: http
slug: crela-io-authentication
source_filename: crela-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://crela.io/docs#rest-api\ndocs: https://crela.io/docs#rest-api\nschemes:\n- type: http\n  scheme: bearer\n  name: Crela API key\n  header: Authorization\n  format: 'Authorization: Bearer crela_<your-api-key>'\n  key_prefix: crela_\n  description: All endpoints except GET /api/agent/requirements require a Bearer token. Keys are created in the creator dashboard (https://crela.io/dashboard/creator/keys); the full key is shown once on creation. No limit on active keys.\n  key_management:\n  - POST /api/agent/keys (create; returns the full key once)\n  - PATCH /api/agent/keys/{id} (rename)\n  - DELETE /api/agent/keys/{id} (revoke; takes effect immediately)\n  env_var: CRELA_API_KEY\nunauthenticated:\n- GET /api/agent/requirements\n- hosted MCP connector https://crela.io/mcp (search only, no API key)\nnote: No OAuth or scopes are documented; the generated OpenAPI declares no securitySchemes, so this profile was read from the\
  \ docs.\n"
source_yaml_url: https://artifacts.apis.io/crela-io/authentication/crela-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Software Marketplace
- Desktop Software
- Independent Creators
- Software Distribution
- Security Review
- MCP
- REST API
---
