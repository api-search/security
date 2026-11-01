---
anonymous_access: false
api_key_in: []
api_specs:
- filename: azion-api-openapi.json
  format: json
  label: azion-api API
  slug: azion-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azion/openapi/_original/azion-api-openapi.json
auth_types: []
description: Authentication schemes for Azion
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Azion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azion declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Azion
provider_slug: azion
scheme_count: 2
schemes:
- evidence: 'Personal token | `Authorization: Token <personal token>` | Agents. Works with the Azion API v4, the MCP servers, and the Azion CLI.'
  header: Authorization
  how_to_obtain: User creates a personal token in Azion Console under Account Menu → Personal Tokens and copies it.
  location: header
  name: TokenAuth
  type: apiKey
- evidence: 'User JWT | `Authorization: Bearer <access_token>` | A session where the user signs in to the Azion API v4 themselves.'
  header: Authorization
  how_to_obtain: User logs in via POST to https://api.azion.com/v4/account/auth/login with email and password to receive an access_token.
  location: header
  name: BearerAuth
  token_url: POST https://api.azion.com/v4/account/auth/login
  type: http-bearer
slug: azion-authentication
source_filename: azion-authentication.yml
source_heading: Authentication Profile
source_url: https://www.azion.com/auth.md
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.azion.com/auth.md\nsources:\n- https://www.azion.com/auth.md\n- https://www.azion.com/en/documentation/fundamentals/personal-tokens/\n- https://www.azion.com/es/blog/como-manejar-trafico-ai-agents-en-apis-rate-limits-auth-observabilidad/\n- https://www.azion.com/pt-br/blog/como-lidar-com-trafego-de-ai-agents-em-apis-rate-limits-auth-observabilidade/\ndescription: Authentication schemes for Azion\nschemes:\n- type: apiKey\n  name: TokenAuth\n  evidence: 'Personal token | `Authorization: Token <personal token>` | Agents. Works with the Azion API v4, the MCP servers, and the Azion CLI.'\n  location: header\n  header: Authorization\n  how_to_obtain: User creates a personal token in Azion Console under Account Menu → Personal Tokens and copies it.\n- type: http-bearer\n  name: BearerAuth\n  evidence: 'User JWT | `Authorization: Bearer <access_token>` | A session where the\
  \ user signs in to the Azion API v4 themselves.'\n  location: header\n  header: Authorization\n  token_url: POST https://api.azion.com/v4/account/auth/login\n  how_to_obtain: User logs in via POST to https://api.azion.com/v4/account/auth/login with email and password to receive an access_token.\ndocs: https://www.azion.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/azion/authentication/azion-authentication.yml
summary_line: 2 schemes
tags:
- Edge Computing
- Serverless
- Artificial Intelligence
- Cloud Infrastructure
- Platform
---
