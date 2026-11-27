---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dazie-io-account-api-openapi.yml
  format: yaml
  label: dazie Account API
  slug: dazie-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-account-api-openapi.yml
- filename: dazie-io-calls-api-openapi.yml
  format: yaml
  label: dazie Calls API
  slug: dazie-io-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-calls-api-openapi.yml
- filename: dazie-io-journal-api-openapi.yml
  format: yaml
  label: dazie Journal API
  slug: dazie-io-journal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-journal-api-openapi.yml
- filename: dazie-io-memories-api-openapi.yml
  format: yaml
  label: dazie Memories API
  slug: dazie-io-memories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-memories-api-openapi.yml
- filename: dazie-io-to-dos-api-openapi.yml
  format: yaml
  label: dazie To Dos API
  slug: dazie-io-to-dos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-to-dos-api-openapi.yml
auth_types: []
description: Authentication schemes for dazie
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: dazie Authentication
name_suffix: Authentication
oauth_flows: []
overview: dazie declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: dazie
provider_slug: dazie-io
scheme_count: 1
schemes:
- evidence: 'How the dazie CLI, SDK, API and MCP server sign in as a user: OAuth 2.1 with PKCE and dynamic client registration.'
  flows:
  - authorization_code
  - refresh_token
  header: Authorization
  how_to_obtain: Register a public client with dynamic client registration (RFC 7591) and use the authorization endpoint with PKCE.
  location: header
  name: OAuth 2.1
  type: oauth2
slug: dazie-io-authentication
source_filename: dazie-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.dazie.io/auth.md
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.dazie.io/auth.md\nsources:\n- https://docs.dazie.io/auth.md\n- https://docs.dazie.io/quickstart.md\ndescription: Authentication schemes for dazie\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: 'How the dazie CLI, SDK, API and MCP server sign in as a user: OAuth 2.1 with PKCE and dynamic client registration.'\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  - refresh_token\n  how_to_obtain: Register a public client with dynamic client registration (RFC 7591) and use the authorization endpoint with PKCE.\ndocs: https://docs.dazie.io/auth.md\n"
source_yaml_url: https://artifacts.apis.io/dazie-io/authentication/dazie-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Voice
- Journaling
- Artificial Intelligence
- Productivity
- Early-Access
---
