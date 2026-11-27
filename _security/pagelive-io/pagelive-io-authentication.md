---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pagelive-io-openapi-generated.yml
  format: yaml
  label: Pagelive API
  slug: pagelive-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelive-io/openapi/_ae-authored/pagelive-io-openapi-generated.yml
auth_types: []
description: Authentication methods for Pagelive MCP API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Pagelive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pagelive declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Pagelive
provider_slug: pagelive-io
scheme_count: 2
schemes:
- evidence: 'Auth, one of: **OAuth** in Claude.ai and Claude Code. Add the URL, then sign in to Pagelive in the browser window that opens.'
  name: OAuth
  type: oauth2
- evidence: 'Send it as `Authorization: Bearer pl_...`. Treat it like a password: anyone holding it can publish to the account.'
  header: Authorization
  how_to_obtain: Create one at https://app.pagelive.io/dashboard/keys (dashboard, "API & MCP"). It is shown once.
  location: header
  name: API key
  type: apiKey
slug: pagelive-io-authentication
source_filename: pagelive-io-authentication.yml
source_heading: Authentication Profile
source_url: https://pagelive.io/agent-setup.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://pagelive.io/agent-setup.md\nsources:\n- https://pagelive.io/agent-setup.md\n- https://pagelive.io/docs/quickstart-mcp\n- https://pagelive.io/docs/getting-started\ndescription: Authentication methods for Pagelive MCP API\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: 'Auth, one of: **OAuth** in Claude.ai and Claude Code. Add the URL, then sign in to Pagelive in the browser window that opens.'\n- type: apiKey\n  name: API key\n  evidence: 'Send it as `Authorization: Bearer pl_...`. Treat it like a password: anyone holding it can publish to the account.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create one at https://app.pagelive.io/dashboard/keys (dashboard, \"API & MCP\"). It is shown once.\ndocs: https://pagelive.io/agent-setup.md\n"
source_yaml_url: https://artifacts.apis.io/pagelive-io/authentication/pagelive-io-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Document Sharing
- Secure Links
- Software-as-a-Service
- Collaboration
---
