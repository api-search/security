---
anonymous_access: false
api_key_in: []
api_specs:
- filename: omnara-com-auth-api-openapi.yml
  format: yaml
  label: Omnara Auth API
  slug: omnara-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omnara-com/openapi/omnara-com-auth-api-openapi.yml
- filename: omnara-com-machines-api-openapi.yml
  format: yaml
  label: Omnara Machines API
  slug: omnara-com-machines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omnara-com/openapi/omnara-com-machines-api-openapi.yml
- filename: omnara-com-relay-api-openapi.yml
  format: yaml
  label: Omnara Relay API
  slug: omnara-com-relay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omnara-com/openapi/omnara-com-relay-api-openapi.yml
- filename: omnara-com-user-sessions-api-openapi.yml
  format: yaml
  label: Omnara User Sessions API
  slug: omnara-com-user-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omnara-com/openapi/omnara-com-user-sessions-api-openapi.yml
- filename: omnara-com-user-settings-api-openapi.yml
  format: yaml
  label: Omnara User Settings API
  slug: omnara-com-user-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omnara-com/openapi/omnara-com-user-settings-api-openapi.yml
- filename: omnara-com-workspaces-api-openapi.yml
  format: yaml
  label: Omnara Workspaces API
  slug: omnara-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omnara-com/openapi/omnara-com-workspaces-api-openapi.yml
- filename: omnara-com-worktrees-api-openapi.yml
  format: yaml
  label: Omnara Worktrees API
  slug: omnara-com-worktrees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omnara-com/openapi/omnara-com-worktrees-api-openapi.yml
auth_types: []
description: Authentication methods for Omnara API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Omnara Authentication
name_suffix: Authentication
oauth_flows: []
overview: Omnara declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Omnara
provider_slug: omnara-com
scheme_count: 2
schemes:
- evidence: Send either key as a bearer token.
  header: Authorization
  how_to_obtain: Create a personal or org API key in the dashboard (Personal tokens page or API Tokens under Access).
  location: header
  name: API Key
  type: http-bearer
- authorize_url: https://app.omnara.com/api/auth/device/code
  evidence: Omnara supports the OAuth 2.0 Device Authorization Grant.
  header: Authorization
  how_to_obtain: Start the flow by POSTing to the device code endpoint with client_id=omnara-cli, then poll the token endpoint for an access token.
  location: header
  name: Device Login
  token_url: https://app.omnara.com/api/auth/device/token
  type: oauth2
slug: omnara-com-authentication
source_filename: omnara-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.omnara.com/api/authentication.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.omnara.com/api/authentication.md\nsources:\n- https://docs.omnara.com/api/authentication.md\n- https://docs.omnara.com/api-reference/endpoints/users-and-api-keys/list-the-authenticated-users-personal-access-tokens.md\n- https://docs.omnara.com/api-reference/endpoints/users-and-api-keys/create-personal-access-token.md\n- https://docs.omnara.com/api-reference/endpoints/users-and-api-keys/revoke-a-personal-access-token.md\ndescription: Authentication methods for Omnara API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Send either key as a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a personal or org API key in the dashboard (Personal tokens page or API Tokens under Access).\n- type: oauth2\n  name: Device Login\n  evidence: Omnara supports the OAuth 2.0 Device Authorization Grant.\n  location: header\n  header: Authorization\n\
  \  token_url: https://app.omnara.com/api/auth/device/token\n  authorize_url: https://app.omnara.com/api/auth/device/code\n  how_to_obtain: Start the flow by POSTing to the device code endpoint with client_id=omnara-cli, then poll the token endpoint for an access token.\ndocs: https://docs.omnara.com/api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/omnara-com/authentication/omnara-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Agents
- Open Source
- Platform
- Automation
---
