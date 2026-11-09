---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ainote-dev-dev-docs-api-openapi.yml
  format: yaml
  label: ainote Dev Docs API
  slug: ainote-dev-dev-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-dev-docs-api-openapi.yml
- filename: ainote-dev-handoffs-api-openapi.yml
  format: yaml
  label: ainote Handoffs API
  slug: ainote-dev-handoffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-handoffs-api-openapi.yml
- filename: ainote-dev-misc-api-openapi.yml
  format: yaml
  label: ainote Misc API
  slug: ainote-dev-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-misc-api-openapi.yml
- filename: ainote-dev-onboarding-api-openapi.yml
  format: yaml
  label: ainote Onboarding API
  slug: ainote-dev-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-onboarding-api-openapi.yml
- filename: ainote-dev-sync-api-openapi.yml
  format: yaml
  label: ainote Sync API
  slug: ainote-dev-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-sync-api-openapi.yml
- filename: ainote-dev-tasks-api-openapi.yml
  format: yaml
  label: ainote Tasks API
  slug: ainote-dev-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-tasks-api-openapi.yml
- filename: ainote-dev-vaults-api-openapi.yml
  format: yaml
  label: ainote Vaults API
  slug: ainote-dev-vaults-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-vaults-api-openapi.yml
auth_types: []
description: Authentication uses API keys sent in the HTTP Authorization header. The header accepts either the prefix “McpKey” or “Bearer” followed by the key value.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ainote Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: ainote declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ainote
provider_slug: ainote-dev
scheme_count: 1
schemes:
- evidence: 'Authorization : McpKey h7Axq9XPsDTD2qr5yqtcCSaQ... Bearer 도 호환 일부 MCP 클라이언트는 Authorization: Bearer ... 만 지원합니다. ainote 는 Bearer 와 McpKey 두 prefix 모두 받습니다.'
  header: Authorization
  how_to_obtain: 키는 signup_and_get_key, login_and_get_key 호출 또는 웹 설정(https://ainote.dev/settings/mcp_keys)에서 발급됩니다.
  location: header
  name: Authorization
  type: apiKey
slug: ainote-dev-authentication
source_filename: ainote-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ainote.dev/guide/auth
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ainote.dev/guide/auth\nsources:\n- https://docs.ainote.dev/guide/auth\n- https://docs.ainote.dev/build/auth\n- https://docs.ainote.dev/reference/auth\n- https://docs.ainote.dev/build/quickstart\ndescription: Authentication uses API keys sent in the HTTP Authorization header. The header accepts either the prefix “McpKey” or “Bearer” followed\n  by the key value.\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'Authorization : McpKey h7Axq9XPsDTD2qr5yqtcCSaQ... Bearer 도 호환 일부 MCP 클라이언트는 Authorization: Bearer ... 만 지원합니다. ainote 는 Bearer 와\n    McpKey 두 prefix 모두 받습니다.'\n  location: header\n  header: Authorization\n  how_to_obtain: 키는 signup_and_get_key, login_and_get_key 호출 또는 웹 설정(https://ainote.dev/settings/mcp_keys)에서 발급됩니다.\nnote: OAuth flows are planned but not currently documented; therefore no OAuth scheme is listed.\ndocs: https://docs.ainote.dev/guide/auth\n"
source_yaml_url: https://artifacts.apis.io/ainote-dev/authentication/ainote-dev-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Productivity
- Note Taking
- Task Management
- Mobile
---
