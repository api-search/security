---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: codebahn-net-activitypub-api-openapi.yml
  format: yaml
  label: Codebahn Activitypub API
  slug: codebahn-net-activitypub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-activitypub-api-openapi.yml
- filename: codebahn-net-admin-api-openapi.yml
  format: yaml
  label: Codebahn Admin API
  slug: codebahn-net-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-admin-api-openapi.yml
- filename: codebahn-net-issue-api-openapi.yml
  format: yaml
  label: Codebahn Issue API
  slug: codebahn-net-issue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-issue-api-openapi.yml
- filename: codebahn-net-miscellaneous-api-openapi.yml
  format: yaml
  label: Codebahn Miscellaneous API
  slug: codebahn-net-miscellaneous-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-miscellaneous-api-openapi.yml
- filename: codebahn-net-notification-api-openapi.yml
  format: yaml
  label: Codebahn Notification API
  slug: codebahn-net-notification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-notification-api-openapi.yml
- filename: codebahn-net-organization-api-openapi.yml
  format: yaml
  label: Codebahn Organization API
  slug: codebahn-net-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-organization-api-openapi.yml
- filename: codebahn-net-package-api-openapi.yml
  format: yaml
  label: Codebahn Package API
  slug: codebahn-net-package-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-package-api-openapi.yml
- filename: codebahn-net-repository-api-openapi.yml
  format: yaml
  label: Codebahn Repository API
  slug: codebahn-net-repository-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-repository-api-openapi.yml
- filename: codebahn-net-settings-api-openapi.yml
  format: yaml
  label: Codebahn Settings API
  slug: codebahn-net-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-settings-api-openapi.yml
- filename: codebahn-net-user-api-openapi.yml
  format: yaml
  label: Codebahn User API
  slug: codebahn-net-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-user-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Codebahn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codebahn secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Codebahn
provider_slug: codebahn-net
scheme_count: 5
schemes:
- description: API tokens must be prepended with "token" followed by a space.
  in: header
  name: AuthorizationHeaderToken
  parameter: Authorization
  sources:
  - openapi/codebahn-net-openapi.yml
  type: apiKey
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/codebahn-net-openapi.yml
  type: http
- description: Sudo API request as the user provided as the key. Admin privileges are required.
  in: header
  name: SudoHeader
  parameter: Sudo
  sources:
  - openapi/codebahn-net-openapi.yml
  type: apiKey
- description: Sudo API request as the user provided as the key. Admin privileges are required.
  in: query
  name: SudoParam
  parameter: sudo
  sources:
  - openapi/codebahn-net-openapi.yml
  type: apiKey
- description: Must be used in combination with BasicAuth if two-factor authentication is enabled.
  in: header
  name: TOTPHeader
  parameter: X-FORGEJO-OTP
  sources:
  - openapi/codebahn-net-openapi.yml
  type: apiKey
slug: codebahn-net-authentication
source_filename: codebahn-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://codebahn.net/docs/cli.md\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: AuthorizationHeaderToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API tokens must be prepended with \"token\" followed by a space.\n  sources:\n  - openapi/codebahn-net-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/codebahn-net-openapi.yml\n- name: SudoHeader\n  type: apiKey\n  in: header\n  parameter: Sudo\n  description: Sudo API request as the user provided as the key. Admin privileges are required.\n  sources:\n  - openapi/codebahn-net-openapi.yml\n- name: SudoParam\n  type: apiKey\n  in: query\n  parameter: sudo\n  description: Sudo API request as the user provided as the key. Admin privileges are required.\n  sources:\n  - openapi/codebahn-net-openapi.yml\n- name: TOTPHeader\n  type: apiKey\n  in: header\n  parameter:\
  \ X-FORGEJO-OTP\n  description: Must be used in combination with BasicAuth if two-factor authentication is enabled.\n  sources:\n  - openapi/codebahn-net-openapi.yml\ndocs: https://codebahn.net/docs/cli.md\ndocumented_flows:\n- name: OAuth (browser)\n  used_by:\n  - CLI (codebahn auth login)\n  - MCP server https://codebahn.net/mcp\n  note: MCP clients must support OAuth discovery and Client ID Metadata Documents; tokens refresh automatically.\n- name: Personal access token\n  note: 'Created under Settings > Applications; sent as Authorization: Bearer for MCP clients without\n    OAuth support, or CODEBAHN_TOKEN / --token for the CLI.'\n- name: Two-factor authentication\n  note: Sign-in uses an emailed code plus optional authenticator passcode or security key; OAuth tokens\n    issued afterwards need no second factor.\ndocs_urls:\n- https://codebahn.net/docs/cli.md\n- https://codebahn.net/docs/mcp.md\n- https://codebahn.net/docs/two-factor-authentication.md\n- https://forgejo.org/docs/v15.0/user/api-usage/#authentication\n"
source_yaml_url: https://artifacts.apis.io/codebahn-net/authentication/codebahn-net-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Company
- Git Hosting
- Version Control
- Continuous Integration
- Forgejo
- Developer Tools
- EU-hosted
- Data Sovereignty
- MCP
---
