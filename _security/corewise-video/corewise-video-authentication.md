---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CoreWise Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoreWise secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CoreWise
provider_slug: corewise-video
scheme_count: 1
schemes:
- description: CoreWise API key created at https://corewise.video/profile under the "API & MCP Keys" card (free account required). Up to 3 active keys; revocation takes effect immediately; rotate by creating a new key, updating the client, then revoking the old one. A key acts as its owner - extractions it starts count toward the owner's monthly quota. The docs state authentication uses only a SHA-256 hash of the key, with an encrypted recoverable copy so it can be re-copied from the Profile.
  format: 'Authorization: Bearer cw_live_...'
  header: Authorization
  in: header
  key_prefix: cw_live_
  name: corewiseApiKey
  optional_for:
  - search_public_extractions
  required_for:
  - extract_url
  - get_extraction (private extractions)
  - get_transcript (private extractions)
  scheme: bearer
  surface: MCP server https://corewise.video/mcp
  type: http
slug: corewise-video-authentication
source_filename: corewise-video-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://corewise.video/docs/features/mcp-server\ndocs: https://corewise.video/docs/features/mcp-server\nsummary:\n  types:\n  - http\nschemes:\n- name: corewiseApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer cw_live_...'\n  key_prefix: cw_live_\n  description: CoreWise API key created at https://corewise.video/profile under the \"API & MCP Keys\" card (free account required). Up to 3 active keys; revocation takes effect immediately; rotate by creating a new key, updating the client, then revoking the old one. A key acts as its owner - extractions it starts count toward the owner's monthly quota. The docs state authentication uses only a SHA-256 hash of the key, with an encrypted recoverable copy so it can be re-copied from the Profile.\n  required_for:\n  - extract_url\n  - get_extraction (private extractions)\n  - get_transcript (private extractions)\n  optional_for:\n\
  \  - search_public_extractions\n  surface: MCP server https://corewise.video/mcp\nnote: Only the MCP server is a public API surface; llms-full.txt states the wider REST API (139+ endpoints) remains internal and is not publicly documented. No OAuth scopes are documented. Invalid key returns HTTP 401 \"Invalid or revoked API key\".\n"
source_yaml_url: https://artifacts.apis.io/corewise-video/authentication/corewise-video-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Video Summarization
- Knowledge Management
- Research
- MCP
- Content Extraction
---
