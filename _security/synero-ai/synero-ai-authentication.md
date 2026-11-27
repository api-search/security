---
anonymous_access: false
api_key_in: []
api_specs:
- filename: synero-ai-api-openapi.json
  format: json
  label: Synero API API
  slug: synero-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synero-ai/openapi/_original/synero-ai-api-openapi.json
auth_types: []
description: Clients authenticate by sending an HTTP Authorization header with a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Synero Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synero declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Synero
provider_slug: synero-ai
scheme_count: 1
schemes:
- evidence: 'curl https://synero.ai/api/query \ -H "Authorization: Bearer sk_live_your_key" \ -H "Content-Type: application/json" \ -d ''{ "prompt": "Postgres or DynamoDB for this service?", "format": "json" }'''
  header: Authorization
  how_to_obtain: Generate an API key in the Synero dashboard (see Connections are scoped to council queries and revocable anytime at synero.ai/app/api-keys). The key is used as a Bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: synero-ai-authentication
source_filename: synero-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://synero.ai/mcp
source_yaml: "generated: '2026-11-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://synero.ai/mcp\nsources:\n- https://synero.ai/mcp\ndescription: Clients authenticate by sending an HTTP Authorization header with a Bearer token.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl https://synero.ai/api/query \\ -H \"Authorization: Bearer sk_live_your_key\" \\ -H \"Content-Type: application/json\" \\ -d ''{ \"prompt\":\n    \"Postgres or DynamoDB for this service?\", \"format\": \"json\" }'''\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the Synero dashboard (see Connections are scoped to council queries and revocable anytime at synero.ai/app/api-keys).\n    The key is used as a Bearer token.\ndocs: https://synero.ai/mcp\n"
source_yaml_url: https://artifacts.apis.io/synero-ai/authentication/synero-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
