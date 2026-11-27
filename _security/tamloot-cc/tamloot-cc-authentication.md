---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tamloot-cc-account-api-openapi.yml
  format: yaml
  label: Tamloot Account API
  slug: tamloot-cc-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-account-api-openapi.yml
- filename: tamloot-cc-changes-api-openapi.yml
  format: yaml
  label: Tamloot Changes API
  slug: tamloot-cc-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-changes-api-openapi.yml
- filename: tamloot-cc-contacts-api-openapi.yml
  format: yaml
  label: Tamloot Contacts API
  slug: tamloot-cc-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-contacts-api-openapi.yml
- filename: tamloot-cc-health-api-openapi.yml
  format: yaml
  label: Tamloot Health API
  slug: tamloot-cc-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-health-api-openapi.yml
- filename: tamloot-cc-me-api-openapi.yml
  format: yaml
  label: Tamloot Me API
  slug: tamloot-cc-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-me-api-openapi.yml
- filename: tamloot-cc-notes-api-openapi.yml
  format: yaml
  label: Tamloot Notes API
  slug: tamloot-cc-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-notes-api-openapi.yml
- filename: tamloot-cc-read-api-api-openapi.yml
  format: yaml
  label: Tamloot Read API
  slug: tamloot-cc-read-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-read-api-api-openapi.yml
- filename: tamloot-cc-service-api-openapi.yml
  format: yaml
  label: Tamloot Service API
  slug: tamloot-cc-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-service-api-openapi.yml
- filename: tamloot-cc-sessions-api-openapi.yml
  format: yaml
  label: Tamloot Sessions API
  slug: tamloot-cc-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-sessions-api-openapi.yml
- filename: tamloot-cc-tasks-api-openapi.yml
  format: yaml
  label: Tamloot Tasks API
  slug: tamloot-cc-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-tasks-api-openapi.yml
auth_types: []
description: 'Tamloot provides two authentication methods: a bearer API key for the public REST API and OAuth 2.1 bearer tokens for the MCP server.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Tamloot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tamloot declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Tamloot
provider_slug: tamloot-cc
scheme_count: 2
schemes:
- evidence: "Send it as a bearer token on every data request:\n\n```bash\ncurl \"https://api.tamloot.cc/v1/contacts?query=maya\" \\\n  -H \"Authorization: Bearer tml_live_your_key\"\n```"
  header: Authorization
  how_to_obtain: A human creates the key in Settings → API in the Tamloot dashboard; the full secret is shown only once.
  location: header
  name: Public REST API bearer API key
  type: http-bearer
- evidence: 'Send the resulting access token as a bearer token on every MCP request:


    ```

    Authorization: Bearer <access_token>

    ```'
  header: Authorization
  how_to_obtain: The client runs an OAuth 2.1 authorization‑code flow with PKCE; a human logs in via the Authorization Server’s login screen and consents, producing an access token.
  location: header
  name: MCP server OAuth 2.1
  type: http-bearer
slug: tamloot-cc-authentication
source_filename: tamloot-cc-authentication.yml
source_heading: Authentication Profile
source_url: https://tamloot.cc/en/docs/developers/api-reference/get-me
source_yaml: "generated: '2026-11-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tamloot.cc/en/docs/developers/api-reference/get-me\nsources:\n- https://tamloot.cc/en/docs/developers/api-reference/get-me\n- https://tamloot.cc/en/docs/developers/quickstart\n- https://tamloot.cc/auth.md\n- https://tamloot.cc/en/docs/developers/mcp-server\ndescription: 'Tamloot provides two authentication methods: a bearer API key for the public REST API and OAuth 2.1 bearer tokens for the MCP server.'\nschemes:\n- type: http-bearer\n  name: Public REST API bearer API key\n  evidence: \"Send it as a bearer token on every data request:\\n\\n```bash\\ncurl \\\"https://api.tamloot.cc/v1/contacts?query=maya\\\" \\\\\\n  -H \\\"Authorization:\\\n    \\ Bearer tml_live_your_key\\\"\\n```\"\n  location: header\n  header: Authorization\n  how_to_obtain: A human creates the key in Settings → API in the Tamloot dashboard; the full secret is shown only once.\n- type: http-bearer\n\
  \  name: MCP server OAuth 2.1\n  evidence: 'Send the resulting access token as a bearer token on every MCP request:\n\n\n    ```\n\n    Authorization: Bearer <access_token>\n\n    ```'\n  location: header\n  header: Authorization\n  how_to_obtain: The client runs an OAuth 2.1 authorization‑code flow with PKCE; a human logs in via the Authorization Server’s login screen and\n    consents, producing an access token.\ndocs: https://tamloot.cc/en/docs/developers/api-reference/get-me\n"
source_yaml_url: https://artifacts.apis.io/tamloot-cc/authentication/tamloot-cc-authentication.yml
summary_line: 2 schemes
tags:
- AI
- CRM
- Business
- Productivity
- Small Business
---
