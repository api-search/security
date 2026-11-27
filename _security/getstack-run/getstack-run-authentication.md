---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getstack-run-openapi-generated.yml
  format: yaml
  label: STACK API
  slug: getstack-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getstack-run/openapi/_ae-authored/getstack-run-openapi-generated.yml
auth_types: []
description: Authentication methods described in STACK documentation
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: STACK Authentication
name_suffix: Authentication
oauth_flows: []
overview: STACK declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: STACK
provider_slug: getstack-run
scheme_count: 4
schemes:
- evidence: 'Authorization Header text Authorization: Bearer $STACK_TOKEN'
  header: Authorization
  location: header
  name: Operator token
  type: http-bearer
- evidence: MCP clients, the CLI and other authorized integrations use short-lived OAuth access tokens.
  header: Authorization
  how_to_obtain: Obtain via OAuth flow as described in MCP setup and discovery endpoints
  location: header
  name: OAuth access token
  type: http-bearer
- evidence: Customer-managed agents enroll a public key and exchange a signed challenge for a short-lived agent JWT.
  header: Authorization
  how_to_obtain: Enroll agent with public key and receive JWT after challenge exchange
  location: header
  name: Agent JWT
  type: http-bearer
- evidence: Send it in X-Passport-Token when a route requires it.
  header: X-Passport-Token
  how_to_obtain: Generated as a passport proving agent identity and delegated scope
  location: header
  name: Passport token
  type: other
slug: getstack-run-authentication
source_filename: getstack-run-authentication.yml
source_heading: Authentication Profile
source_url: https://getstack.run/docs/api/authentication
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getstack.run/docs/api/authentication\nsources:\n- https://getstack.run/docs/api/authentication\n- https://getstack.run/docs/security/mcp-auth-troubleshooting\n- https://getstack.run/docs/getting-started\n- https://getstack.run/docs/security/mcp-setup\ndescription: Authentication methods described in STACK documentation\nschemes:\n- type: http-bearer\n  name: Operator token\n  evidence: 'Authorization Header text Authorization: Bearer $STACK_TOKEN'\n  location: header\n  header: Authorization\n- type: http-bearer\n  name: OAuth access token\n  evidence: MCP clients, the CLI and other authorized integrations use short-lived OAuth access tokens.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain via OAuth flow as described in MCP setup and discovery endpoints\n- type: http-bearer\n  name: Agent JWT\n  evidence: Customer-managed agents enroll a public key\
  \ and exchange a signed challenge for a short-lived agent JWT.\n  location: header\n  header: Authorization\n  how_to_obtain: Enroll agent with public key and receive JWT after challenge exchange\n- type: other\n  name: Passport token\n  evidence: Send it in X-Passport-Token when a route requires it.\n  location: header\n  header: X-Passport-Token\n  how_to_obtain: Generated as a passport proving agent identity and delegated scope\nnote: OAuth flow details (authorize/token URLs, scopes) are not explicitly listed in the provided pages, so they are omitted. 1 extracted row(s)\n  were dropped because their quote was not on the page.\ndocs: https://getstack.run/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/getstack-run/authentication/getstack-run-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Artificial Intelligence
- Security
- Identity
- Compliance
---
