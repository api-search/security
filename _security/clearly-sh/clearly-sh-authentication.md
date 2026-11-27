---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clearly-sh-openapi-generated.yml
  format: yaml
  label: Clearly API
  slug: clearly-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearly-sh/openapi/_ae-authored/clearly-sh-openapi-generated.yml
auth_types: []
description: Authentication is performed via OAuth sign‑in in the browser. The client opens a browser to the MCP endpoint and the user selects a workspace and agent. Scopes are rpc:read, rpc:write, rpc:admin.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Clearly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clearly declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Clearly
provider_slug: clearly-sh
scheme_count: 1
schemes:
- evidence: Sign in through OAuth; no coding runtime is required.
  how_to_obtain: Run the client command (e.g., `claude mcp login clearly` or `beehaven login`) which opens a browser for the user to complete the OAuth sign‑in.
  name: OAuth
  scopes:
  - rpc:read
  - rpc:write
  - rpc:admin
  type: oauth2
slug: clearly-sh-authentication
source_filename: clearly-sh-authentication.yml
source_heading: Authentication Profile
source_url: https://www.clearly.sh/setup.md
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.clearly.sh/setup.md\nsources:\n- https://www.clearly.sh/setup.md\n- https://www.clearly.sh/docs/mcp\n- https://www.clearly.sh/docs/quickstart\n- https://www.clearly.sh/docs/shopify\ndescription: Authentication is performed via OAuth sign‑in in the browser. The client opens a browser to the MCP endpoint and the user selects\n  a workspace and agent. Scopes are rpc:read, rpc:write, rpc:admin.\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Sign in through OAuth; no coding runtime is required.\n  scopes:\n  - rpc:read\n  - rpc:write\n  - rpc:admin\n  how_to_obtain: Run the client command (e.g., `claude mcp login clearly` or `beehaven login`) which opens a browser for the user to complete\n    the OAuth sign‑in.\ndocs: https://www.clearly.sh/setup.md\n"
source_yaml_url: https://artifacts.apis.io/clearly-sh/authentication/clearly-sh-authentication.yml
summary_line: 1 scheme
tags:
- AI Agents
- Workspace
- Design Tools
---
