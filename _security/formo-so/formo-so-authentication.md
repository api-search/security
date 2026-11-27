---
anonymous_access: false
api_key_in: []
api_specs:
- filename: formo-so-alerts-api-openapi.yml
  format: yaml
  label: Formo Alerts API
  slug: formo-so-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-alerts-api-openapi.yml
- filename: formo-so-boards-api-openapi.yml
  format: yaml
  label: Formo Boards API
  slug: formo-so-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-boards-api-openapi.yml
- filename: formo-so-charts-api-openapi.yml
  format: yaml
  label: Formo Charts API
  slug: formo-so-charts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-charts-api-openapi.yml
- filename: formo-so-contracts-api-openapi.yml
  format: yaml
  label: Formo Contracts API
  slug: formo-so-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-contracts-api-openapi.yml
- filename: formo-so-events-api-openapi.yml
  format: yaml
  label: Formo Events API
  slug: formo-so-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-events-api-openapi.yml
- filename: formo-so-profiles-api-openapi.yml
  format: yaml
  label: Formo Profiles API
  slug: formo-so-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-profiles-api-openapi.yml
- filename: formo-so-query-api-openapi.yml
  format: yaml
  label: Formo Query API
  slug: formo-so-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-query-api-openapi.yml
- filename: formo-so-segments-api-openapi.yml
  format: yaml
  label: Formo Segments API
  slug: formo-so-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-segments-api-openapi.yml
auth_types: []
description: Formo API authentication uses API keys sent as Bearer tokens in the Authorization header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Formo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Formo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Formo
provider_slug: formo-so
scheme_count: 2
schemes:
- evidence: 'To access the Profiles and Query API, include your workspace API key in your request headers as a Bearer token: Authorization: Bearer < your_workspace_api_key >'
  header: Authorization
  how_to_obtain: Find your API key in your workspace settings. Create one with the appropriate scope if you don’t have one yet.
  name: Workspace API Key
  scopes:
  - profiles:read
  - profiles:write
  - query:read
  - alerts:read
  - alerts:write
  - boards:read
  - boards:write
  - contracts:read
  - contracts:write
  - segments:read
  - segments:write
  type: http-bearer
- evidence: 'To send events through the Events API, include the SDK Write Key in your request headers: Authorization: Bearer < token >'
  header: Authorization
  how_to_obtain: Find your SDK Write Key in your project settings.
  name: SDK Write Key
  type: http-bearer
slug: formo-so-authentication
source_filename: formo-so-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.formo.so/api/authentication
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.formo.so/api/authentication\nsources:\n- https://docs.formo.so/api/authentication\ndescription: Formo API authentication uses API keys sent as Bearer tokens in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Workspace API Key\n  evidence: 'To access the Profiles and Query API, include your workspace API key in your request headers as a Bearer token: Authorization: Bearer\n    < your_workspace_api_key >'\n  header: Authorization\n  scopes:\n  - profiles:read\n  - profiles:write\n  - query:read\n  - alerts:read\n  - alerts:write\n  - boards:read\n  - boards:write\n  - contracts:read\n  - contracts:write\n  - segments:read\n  - segments:write\n  how_to_obtain: Find your API key in your workspace settings. Create one with the appropriate scope if you don’t have one yet.\n- type: http-bearer\n  name: SDK Write Key\n  evidence: 'To send events through the\
  \ Events API, include the SDK Write Key in your request headers: Authorization: Bearer < token >'\n  header: Authorization\n  how_to_obtain: Find your SDK Write Key in your project settings.\ndocs: https://docs.formo.so/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/formo-so/authentication/formo-so-authentication.yml
summary_line: 2 schemes
tags:
- Analytics
- Attribution
- Cryptocurrency
- DeFi
- Wallet Intelligence
- Token‑Gated Forms
- AI Agents
---
