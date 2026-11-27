---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Reeling REST API and MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Reeling Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reeling declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Reeling
provider_slug: reeling-app
scheme_count: 2
schemes:
- evidence: 'Authenticate by passing X-API-Key: rl_live_... or Authorization: Bearer rl_live_... in request headers—never in URL query parameters where keys leak into proxy and analytics logs.'
  header: X-API-Key
  how_to_obtain: Generate dedicated keys in Settings → API & Automation for each agent runtime.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'Authenticate by passing X-API-Key: rl_live_... or Authorization: Bearer rl_live_... in request headers—never in URL query parameters where keys leak into proxy and analytics logs.'
  header: Authorization
  how_to_obtain: Generate dedicated keys in Settings → API & Automation for each agent runtime.
  location: header
  name: Authorization
  type: http-bearer
slug: reeling-app-authentication
source_filename: reeling-app-authentication.yml
source_heading: Authentication Profile
source_url: https://reeling.app/developers/security.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://reeling.app/developers/security.md\nsources:\n- https://reeling.app/developers/security.md\n- https://reeling.app/developers/api\n- https://reeling.app/blog/threads-api-guide-post-tokens-rate-limits.md\n- https://reeling.app/developers/mcp.md\ndescription: Authentication methods for Reeling REST API and MCP\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Authenticate by passing X-API-Key: rl_live_... or Authorization: Bearer rl_live_... in request headers—never in URL query parameters\n    where keys leak into proxy and analytics logs.'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Generate dedicated keys in Settings → API & Automation for each agent runtime.\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authenticate by passing X-API-Key: rl_live_... or Authorization: Bearer rl_live_... in request headers—never in URL query parameters\n\
  \    where keys leak into proxy and analytics logs.'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate dedicated keys in Settings → API & Automation for each agent runtime.\ndocs: https://reeling.app/developers/security.md\n"
source_yaml_url: https://artifacts.apis.io/reeling-app/authentication/reeling-app-authentication.yml
summary_line: 2 schemes
tags:
- Video Scheduling
- AI Content Generation
- Multi-Channel Publishing
- Developer Tools
- Creator Tools
---
