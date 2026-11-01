---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tinycommand-account-openapi-generated.yml
  format: yaml
  label: TinyCommand Account & Workspace 9 articles Manage your workspace, team members, credits, bil API
  slug: account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinycommand/openapi/_ae-authored/tinycommand-account-openapi-generated.yml
- filename: tinycommand-core-openapi-generated.yml
  format: yaml
  label: TinyCommand core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinycommand/openapi/_ae-authored/tinycommand-core-openapi-generated.yml
- filename: tinycommand-mcp-openapi-generated.yml
  format: yaml
  label: TinyCommand MCP Server 9 articles Drive your Tiny Command workspace from Claude Desktop, Cur API
  slug: mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinycommand/openapi/_ae-authored/tinycommand-mcp-openapi-generated.yml
- filename: tinycommand-tables-openapi-generated.yml
  format: yaml
  label: TinyCommand TinyTables 40 articles Spreadsheet-database hybrid, with 37 column types, six vi API
  slug: tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinycommand/openapi/_ae-authored/tinycommand-tables-openapi-generated.yml
- filename: tinycommand-workflows-openapi-generated.yml
  format: yaml
  label: TinyCommand TinyWorkflows 96 articles Visual automation builder. Connect apps, add logic, an API
  slug: workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinycommand/openapi/_ae-authored/tinycommand-workflows-openapi-generated.yml
auth_types: []
description: Authentication methods for TinyCommand
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Tinycommand Authentication
name_suffix: Authentication
oauth_flows: []
overview: TinyCommand declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: TinyCommand
provider_slug: tinycommand
scheme_count: 2
schemes:
- evidence: Every request to the Tiny Command MCP server is authenticated with a workspace API key sent as a bearer token.
  header: Authorization
  how_to_obtain: Generate, list, and revoke keys in the platform under MCP keys. Issuing keys requires a workspace Admin or Owner role.
  location: header
  name: Workspace API Key
  type: http-bearer
- evidence: When a respondent reaches this field, they see a button to connect their account via OAuth -- they click it, sign in to the service, grant permissions, and return to the form with a valid authorization token stored in the submission.
  name: Connection field OAuth
  type: oauth2
slug: tinycommand-authentication
source_filename: tinycommand-authentication.yml
source_heading: Authentication Profile
source_url: https://tinycommand.com/docs/forms/fields/connection
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tinycommand.com/docs/forms/fields/connection\nsources:\n- https://tinycommand.com/docs/forms/fields/connection\n- https://tinycommand.com/docs/mcp/authentication\n- https://tinycommand.com/docs/account/api-keys\n- https://tinycommand.com/docs/forms/getting-started\ndescription: Authentication methods for TinyCommand\nschemes:\n- type: http-bearer\n  name: Workspace API Key\n  evidence: Every request to the Tiny Command MCP server is authenticated with a workspace API key sent as a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate, list, and revoke keys in the platform under MCP keys. Issuing keys requires a workspace Admin or Owner role.\n- type: oauth2\n  name: Connection field OAuth\n  evidence: When a respondent reaches this field, they see a button to connect their account via OAuth -- they click it, sign in to the service,\n    grant\
  \ permissions, and return to the form with a valid authorization token stored in the submission.\ndocs: https://tinycommand.com/docs/forms/fields/connection\n"
source_yaml_url: https://artifacts.apis.io/tinycommand/authentication/tinycommand-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Recruiting
- Automation
- Software-as-a-Service
- Artificial Intelligence
---
