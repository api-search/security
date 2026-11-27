---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for Frontshelf APIs uses a bearer token called an Agent key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Frontshelf Authentication
name_suffix: Authentication
oauth_flows: []
overview: Frontshelf declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Frontshelf
provider_slug: frontshelf-io
scheme_count: 1
schemes:
- evidence: MCP server POST /mcp , Agent-key bearer auth, one tool ( frontshelf )
  header: Authorization
  how_to_obtain: Create an Agent key via the Frontshelf portal or using the `frontshelf login` command.
  location: header
  name: Agent-key
  type: http-bearer
slug: frontshelf-io-authentication
source_filename: frontshelf-io-authentication.yml
source_heading: Authentication Profile
source_url: https://frontshelf.io/docs
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://frontshelf.io/docs\nsources:\n- https://frontshelf.io/docs\ndescription: Authentication for Frontshelf APIs uses a bearer token called an Agent key.\nschemes:\n- type: http-bearer\n  name: Agent-key\n  evidence: MCP server POST /mcp , Agent-key bearer auth, one tool ( frontshelf )\n  location: header\n  header: Authorization\n  how_to_obtain: Create an Agent key via the Frontshelf portal or using the `frontshelf login` command.\nnote: The same bearer token is used for the REST API (/api/v1) as indicated in the documentation.\ndocs: https://frontshelf.io/docs\n"
source_yaml_url: https://artifacts.apis.io/frontshelf-io/authentication/frontshelf-io-authentication.yml
summary_line: 1 scheme
tags:
- Technical SEO
---
