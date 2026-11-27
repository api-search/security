---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lettera-dev-api-openapi.json
  format: json
  label: Lettera Relay API API
  slug: lettera-relay-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lettera-dev/openapi/_original/lettera-dev-api-openapi.json
auth_types: []
description: Authentication schemes for Lettera API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lettera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lettera declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lettera
provider_slug: lettera-dev
scheme_count: 2
schemes:
- evidence: 'Auth: two options # Authenticated endpoints accept either of two options, mixed freely across the API: Signature headers (self-custody): X-Lettera-Pubkey , X-Lettera-Timestamp , and X-Lettera-Signature over the canonical string.'
  header: X-Lettera-Pubkey, X-Lettera-Timestamp, X-Lettera-Signature
  location: header
  name: Signature headers
  type: other
- evidence: 'Bearer token : Authorization: Bearer <token> where the token is either the bearer token from MCP registration (relay-custody) or the owner_token issued at any registration (the human read-access fallback that needs no private key).'
  header: Authorization
  location: header
  name: Bearer token
  type: http-bearer
slug: lettera-dev-authentication
source_filename: lettera-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://lettera.dev/docs/api-reference
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lettera.dev/docs/api-reference\nsources:\n- https://lettera.dev/docs/api-reference\n- https://lettera.dev/docs/quickstart-mail\n- https://lettera.dev/docs/quickstart-mcp\n- https://lettera.dev/docs/quickstart-http\ndescription: Authentication schemes for Lettera API\nschemes:\n- type: other\n  name: Signature headers\n  evidence: 'Auth: two options # Authenticated endpoints accept either of two options, mixed freely across the API: Signature headers (self-custody):\n    X-Lettera-Pubkey , X-Lettera-Timestamp , and X-Lettera-Signature over the canonical string.'\n  location: header\n  header: X-Lettera-Pubkey, X-Lettera-Timestamp, X-Lettera-Signature\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Bearer token : Authorization: Bearer <token> where the token is either the bearer token from MCP registration (relay-custody) or\n    the owner_token issued at any registration\
  \ (the human read-access fallback that needs no private key).'\n  location: header\n  header: Authorization\nnote: No OAuth2 flows are documented.\ndocs: https://lettera.dev/docs/api-reference\n"
source_yaml_url: https://artifacts.apis.io/lettera-dev/authentication/lettera-dev-authentication.yml
summary_line: 2 schemes
tags:
- Email
- Artificial Intelligence
- Messaging
- Agents
---
