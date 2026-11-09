---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for ContentIn MCP server
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Contentin Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: ContentIn declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ContentIn
provider_slug: contentin-io
scheme_count: 2
schemes:
- evidence: The key goes in the X-MCP-Key header on every request.
  header: X-MCP-Key
  how_to_obtain: Create a key in ContentIn Settings → Connections → "Connect AI clients"; the key starts with cimcp_ and is shown once.
  location: header
  name: X-MCP-Key
  type: apiKey
- evidence: Your client opens a ContentIn sign‑in page in your browser. You log in (or are already logged in) and pick which ContentIn profile this connection acts as.
  how_to_obtain: User authenticates via the ContentIn sign‑in page; no client‑side token or URL is documented.
  name: ContentIn sign‑in
  type: oauth2
slug: contentin-io-authentication
source_filename: contentin-io-authentication.yml
source_heading: Authentication Profile
source_url: https://contentin.io/linkedin-mcp-server/setup/
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://contentin.io/linkedin-mcp-server/setup/\nsources:\n- https://contentin.io/linkedin-mcp-server/setup/\n- https://contentin.io/blog/how-do-i-get-started-with-linkedin-mcp-server/\ndescription: Authentication for ContentIn MCP server\nschemes:\n- type: apiKey\n  name: X-MCP-Key\n  evidence: The key goes in the X-MCP-Key header on every request.\n  location: header\n  header: X-MCP-Key\n  how_to_obtain: Create a key in ContentIn Settings → Connections → \"Connect AI clients\"; the key starts with cimcp_ and is shown once.\n- type: oauth2\n  name: ContentIn sign‑in\n  evidence: Your client opens a ContentIn sign‑in page in your browser. You log in (or are already logged in) and pick which ContentIn profile\n    this connection acts as.\n  how_to_obtain: User authenticates via the ContentIn sign‑in page; no client‑side token or URL is documented.\ndocs: https://contentin.io/linkedin-mcp-server/setup/\n"
source_yaml_url: https://artifacts.apis.io/contentin-io/authentication/contentin-io-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- LinkedIn
- Ghostwriter
- Content Creation
- Software-as-a-Service
- Company
---
