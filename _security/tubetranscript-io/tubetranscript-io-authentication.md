---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses a Pro plan API key passed as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tubetranscript Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: tubetranscript-io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: tubetranscript-io
provider_slug: tubetranscript-io
scheme_count: 2
schemes:
- evidence: 'Send POST https://tubetranscript.io/api/v1/extract with Authorization: Bearer <API_KEY> and a JSON body containing url.'
  header: Authorization
  how_to_obtain: Create a Pro plan API key in the dashboard at /dashboard/api; keys start with tt_live_ followed by 32 characters.
  location: header
  name: Bearer
  type: http-bearer
- evidence: 'Connect an MCP‑capable client to https://tubetranscript.io/api/mcp using the Streamable HTTP transport and the header Authorization: Bearer <API_KEY>.'
  header: Authorization
  how_to_obtain: Create a Pro plan API key in the dashboard at /dashboard/api; keys start with tt_live_ followed by 32 characters.
  location: header
  name: Bearer
  type: http-bearer
slug: tubetranscript-io-authentication
source_filename: tubetranscript-io-authentication.yml
source_heading: Authentication Profile
source_url: https://tubetranscript.io/docs/quickstart.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tubetranscript.io/docs/quickstart.md\nsources:\n- https://tubetranscript.io/docs/quickstart.md\n- https://tubetranscript.io/docs/mcp.md\n- https://tubetranscript.io/docs/quickstart\n- https://tubetranscript.io/docs/mcp\ndescription: Authentication uses a Pro plan API key passed as a Bearer token.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send POST https://tubetranscript.io/api/v1/extract with Authorization: Bearer <API_KEY> and a JSON body containing url.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a Pro plan API key in the dashboard at /dashboard/api; keys start with tt_live_ followed by 32 characters.\n- type: http-bearer\n  name: Bearer\n  evidence: 'Connect an MCP‑capable client to https://tubetranscript.io/api/mcp using the Streamable HTTP transport and the header Authorization:\n    Bearer <API_KEY>.'\n  location: header\n\
  \  header: Authorization\n  how_to_obtain: Create a Pro plan API key in the dashboard at /dashboard/api; keys start with tt_live_ followed by 32 characters.\nnote: Both the REST API and MCP servers use the same Bearer token scheme.\ndocs: https://tubetranscript.io/docs/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/tubetranscript-io/authentication/tubetranscript-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- YouTube
- Transcript
- FreeTool
- API
---
