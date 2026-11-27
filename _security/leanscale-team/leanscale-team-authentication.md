---
anonymous_access: false
api_key_in: []
api_specs:
- filename: leanscale-team-access-api-openapi.yml
  format: yaml
  label: LeanScale Access API
  slug: leanscale-team-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leanscale-team/openapi/leanscale-team-access-api-openapi.yml
- filename: leanscale-team-mcp-api-openapi.yml
  format: yaml
  label: LeanScale MCP API
  slug: leanscale-team-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leanscale-team/openapi/leanscale-team-mcp-api-openapi.yml
auth_types: []
description: LeanScale MCP uses a key for authentication, which can be sent as a bearer token in the Authorization header or as a query parameter named "key".
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LeanScale Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeanScale declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LeanScale
provider_slug: leanscale-team
scheme_count: 2
schemes:
- evidence: under the hood it’s streamable HTTP and JSON‑RPC 2.0 at https://mcp.leanscale.team/mcp, with the key as a bearer token or a ?key= parameter.
  header: Authorization
  how_to_obtain: Obtain a free key by providing a work email on the LeanScale MCP page.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: under the hood it’s streamable HTTP and JSON‑RPC 2.0 at https://mcp.leanscale.team/mcp, with the key as a bearer token or a ?key= parameter.
  how_to_obtain: Obtain a free key by providing a work email on the LeanScale MCP page.
  location: query
  name: Query key
  type: apiKey
slug: leanscale-team-authentication
source_filename: leanscale-team-authentication.yml
source_heading: Authentication Profile
source_url: https://www.leanscale.team/mcp
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.leanscale.team/mcp\nsources:\n- https://www.leanscale.team/mcp\n- https://www.leanscale.team/knowledge/podcast/anish-chadalavada-gradial-the-token-bill-came-due/index.md\n- https://www.leanscale.team/knowledge/playbooks/onboarding-playbook/index.md\n- https://www.leanscale.team/knowledge/docs/getting-started-quickstart/index.md\ndescription: LeanScale MCP uses a key for authentication, which can be sent as a bearer token in the Authorization header or as a query parameter\n  named \"key\".\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: under the hood it’s streamable HTTP and JSON‑RPC 2.0 at https://mcp.leanscale.team/mcp, with the key as a bearer token or a ?key=\n    parameter.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a free key by providing a work email on the LeanScale MCP page.\n- type: apiKey\n  name: Query key\n \
  \ evidence: under the hood it’s streamable HTTP and JSON‑RPC 2.0 at https://mcp.leanscale.team/mcp, with the key as a bearer token or a ?key=\n    parameter.\n  location: query\n  how_to_obtain: Obtain a free key by providing a work email on the LeanScale MCP page.\nnote: No OAuth2 or other authentication methods are documented on the provided pages.\ndocs: https://www.leanscale.team/mcp\n"
source_yaml_url: https://artifacts.apis.io/leanscale-team/authentication/leanscale-team-authentication.yml
summary_line: 2 schemes
tags:
- Go-To-Market
- Revenue Operations
- Software-as-a-Service
- AI-native
- Consulting
---
