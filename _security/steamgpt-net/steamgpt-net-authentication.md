---
anonymous_access: true
api_key_in: []
api_specs:
- filename: steamgpt-net-bans-api-openapi.yml
  format: yaml
  label: steamgpt-net Bans API
  slug: steamgpt-net-bans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-bans-api-openapi.yml
- filename: steamgpt-net-batch-api-openapi.yml
  format: yaml
  label: steamgpt-net Batch API
  slug: steamgpt-net-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-batch-api-openapi.yml
- filename: steamgpt-net-compare-api-openapi.yml
  format: yaml
  label: steamgpt-net Compare API
  slug: steamgpt-net-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-compare-api-openapi.yml
- filename: steamgpt-net-converter-api-openapi.yml
  format: yaml
  label: steamgpt-net Converter API
  slug: steamgpt-net-converter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-converter-api-openapi.yml
- filename: steamgpt-net-faceit-api-openapi.yml
  format: yaml
  label: steamgpt-net Faceit API
  slug: steamgpt-net-faceit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-faceit-api-openapi.yml
- filename: steamgpt-net-friends-api-openapi.yml
  format: yaml
  label: steamgpt-net Friends API
  slug: steamgpt-net-friends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-friends-api-openapi.yml
- filename: steamgpt-net-identity-api-openapi.yml
  format: yaml
  label: steamgpt-net Identity API
  slug: steamgpt-net-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-identity-api-openapi.yml
- filename: steamgpt-net-profile-api-openapi.yml
  format: yaml
  label: steamgpt-net Profile API
  slug: steamgpt-net-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-profile-api-openapi.yml
- filename: steamgpt-net-ready-api-openapi.yml
  format: yaml
  label: steamgpt-net Ready API
  slug: steamgpt-net-ready-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-ready-api-openapi.yml
- filename: steamgpt-net-summary-api-openapi.yml
  format: yaml
  label: steamgpt-net Summary API
  slug: steamgpt-net-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-summary-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Steamgpt Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: steamgpt-net declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: steamgpt-net
provider_slug: steamgpt-net
scheme_count: 2
schemes:
- description: Anonymous access, no credentials required for all endpoints.
  type: none
- bearerFormat: JWT
  description: Optional boost token (client_credentials) that raises rate limit.
  scheme: bearer
  scopes:
  - rate-boost
  type: http
slug: steamgpt-net-authentication
source_filename: steamgpt-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://steamgpt.net/auth.md\nschemes:\n  - type: none\n    description: Anonymous access, no credentials required for all endpoints.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Optional boost token (client_credentials) that raises rate limit.\n    scopes:\n      - rate-boost\n"
source_yaml_url: https://artifacts.apis.io/steamgpt-net/authentication/steamgpt-net-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Steam
- Gaming
- AI
- OpenData
- NoAuth
- Profiles
- Friends
- FACEIT
---
