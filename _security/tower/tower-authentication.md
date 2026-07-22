---
api_key_in:
- header
api_specs:
- filename: tower-openapi-original.json
  format: json
  label: Tower API
  slug: tower-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tower/refs/heads/main/openapi/tower-openapi-original.json
auth_types:
- apiKey
- http-bearer
description: 'Tower API authentication profile, from the OpenAPI securitySchemes and the API-keys documentation. Two schemes: an API key in the X-API-Key header (keys are prefixed sk-, created in Team Settings or via the create-api-key operation, and can be scoped down with the documented permission scopes — see scopes/tower-scopes.yml), and a Bearer access token issued as part of a Tower session (create-session / refresh-session; the CLI logs in via a device-login flow). Service accounts can mint their own API keys (create-service-account-api-key, team admin only). The describe-whoami operation returns an RS256-signed identity JWT verifiable against the JWKS at https://api.tower.dev/.well-known/jwks.json.'
kind: authentication
layout: security
method: searched
name: Tower Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tower secures its APIs with apiKey and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tower
provider_slug: tower
scheme_count: 2
schemes:
- description: API key created by a Tower user or Tower service account to authenticate an API request. Keys are prefixed sk- and default to the creating account's role; pass `scopes` to create-api-key to mint a reduced-privilege key. Wrong/missing scope returns 403 Forbidden.
  in: header
  name: APIKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/tower-openapi-original.json
  type: apiKey
- description: Access token provided by the Tower API as part of a Tower session (see create-session, refresh-session, and the device-login operations).
  name: AccessTokenAuth
  scheme: bearer
  sources:
  - openapi/tower-openapi-original.json
  type: http
slug: tower-authentication
source_filename: tower-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tower.dev/docs/using-tower/api-keys\nspec_source: openapi/tower-openapi-original.json\ndescription: >-\n  Tower API authentication profile, from the OpenAPI securitySchemes and the\n  API-keys documentation. Two schemes: an API key in the X-API-Key header\n  (keys are prefixed sk-, created in Team Settings or via the create-api-key\n  operation, and can be scoped down with the documented permission scopes —\n  see scopes/tower-scopes.yml), and a Bearer access token issued as part of a\n  Tower session (create-session / refresh-session; the CLI logs in via a\n  device-login flow). Service accounts can mint their own API keys\n  (create-service-account-api-key, team admin only). The describe-whoami\n  operation returns an RS256-signed identity JWT verifiable against the JWKS\n  at https://api.tower.dev/.well-known/jwks.json.\nsummary:\n  types: [apiKey, http-bearer]\n  api_key_in: [header]\n  api_key_header: X-API-Key\n\
  \  api_key_prefix: sk-\n  oauth2_flows: []\nschemes:\n  - name: APIKeyAuth\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    description: >-\n      API key created by a Tower user or Tower service account to authenticate\n      an API request. Keys are prefixed sk- and default to the creating\n      account's role; pass `scopes` to create-api-key to mint a\n      reduced-privilege key. Wrong/missing scope returns 403 Forbidden.\n    sources: [openapi/tower-openapi-original.json]\n  - name: AccessTokenAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Access token provided by the Tower API as part of a Tower session (see\n      create-session, refresh-session, and the device-login operations).\n    sources: [openapi/tower-openapi-original.json]\ndocs: https://docs.tower.dev/docs/using-tower/api-keys\nscopes_reference: scopes/tower-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tower/refs/heads/main/authentication/tower-authentication.yml
summary_line: apiKey/http-bearer · 2 schemes
tags:
- Data Infrastructure
- Data Engineering
- Python
- Apache Iceberg
- Lakehouse
- Orchestration
- Data Pipelines
- AI Agents
- MCP
- ETL
---
