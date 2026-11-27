---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for iMario MCP server
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: iMario Authentication
name_suffix: Authentication
oauth_flows: []
overview: iMario declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: iMario
provider_slug: imario-ai
scheme_count: 2
schemes:
- evidence: TRAE sends a fixed header instead of signing in, so it connects with the workspace API key. Ask the user to create the key in iMario (Settings > MCP & API, owners and admins), then to add this in TRAE's MCP window (Add > Add Manually) with the key in place of the placeholder.
  header: Authorization
  how_to_obtain: User creates an API key in iMario settings and provides it to the client.
  location: header
  name: Workspace API Key
  type: http-bearer
- evidence: 'Any other host: a Streamable HTTP server at that address, no headers. It answers 401 with the OAuth discovery documents, and the host takes it from there.'
  how_to_obtain: Client receives 401 response with discovery documents and follows the OAuth flow as defined by the server.
  name: OAuth Discovery
  type: oauth2
slug: imario-ai-authentication
source_filename: imario-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://imario.ai/SKILL.md
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://imario.ai/SKILL.md\nsources:\n- https://imario.ai/SKILL.md\n- https://imario.ai/docs/getting-started/overview.md\n- https://imario.ai/docs/getting-started/quickstart.md\n- https://imario.ai/docs/getting-started/core-concepts.md\ndescription: Authentication methods for iMario MCP server\nschemes:\n- type: http-bearer\n  name: Workspace API Key\n  evidence: TRAE sends a fixed header instead of signing in, so it connects with the workspace API key. Ask the user to create the key in iMario\n    (Settings > MCP & API, owners and admins), then to add this in TRAE's MCP window (Add > Add Manually) with the key in place of the placeholder.\n  location: header\n  header: Authorization\n  how_to_obtain: User creates an API key in iMario settings and provides it to the client.\n- type: oauth2\n  name: OAuth Discovery\n  evidence: 'Any other host: a Streamable HTTP server at that address,\
  \ no headers. It answers 401 with the OAuth discovery documents, and the\n    host takes it from there.'\n  how_to_obtain: Client receives 401 response with discovery documents and follows the OAuth flow as defined by the server.\ndocs: https://imario.ai/SKILL.md\n"
source_yaml_url: https://artifacts.apis.io/imario-ai/authentication/imario-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- SyntheticAudiences
- Marketing
- Data
---
