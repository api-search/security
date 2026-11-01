---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for MemorySync
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Memorysync Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: memorysync-io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: memorysync-io
provider_slug: memorysync-io
scheme_count: 2
schemes:
- evidence: X-API-Key Authenticates your server.
  name: X-API-Key
  type: apiKey
- evidence: Authentication Bearer access token for an active organization member.
  name: Bearer
  type: http-bearer
slug: memorysync-io-authentication
source_filename: memorysync-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.memorysync.io/getting-started/authentication
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.memorysync.io/getting-started/authentication\nsources:\n- https://docs.memorysync.io/getting-started/authentication\n- https://docs.memorysync.io/api/api-keys/bulk-revoke\n- https://docs.memorysync.io/api/api-keys/test\n- https://docs.memorysync.io/api/auth\ndescription: Authentication schemes for MemorySync\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: X-API-Key Authenticates your server.\n- type: http-bearer\n  name: Bearer\n  evidence: Authentication Bearer access token for an active organization member.\nnote: No OAuth2 flows are documented; only API‑key and bearer token methods are described.\ndocs: https://docs.memorysync.io/getting-started/authentication\n"
source_yaml_url: https://artifacts.apis.io/memorysync-io/authentication/memorysync-io-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Memory
- Infrastructure
- Platform
- DeveloperTools
- Company
---
