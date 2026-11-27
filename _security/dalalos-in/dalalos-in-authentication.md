---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dalalos-in-openapi-generated.yml
  format: yaml
  label: DalalOS API
  slug: dalalos-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dalalos-in/openapi/_ae-authored/dalalos-in-openapi-generated.yml
auth_types: []
description: Authentication methods for DalalOS
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: DalalOS Authentication
name_suffix: Authentication
oauth_flows: []
overview: DalalOS declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DalalOS
provider_slug: dalalos-in
scheme_count: 2
schemes:
- evidence: Authorize once A sign-in window opens (Google or email code). Approve it, and Claude is connected. This sign-in standard is called OAuth.
  name: OAuth
  type: oauth2
- evidence: 'Send an API key from your dashboard as Authorization: Bearer isk_live_… .'
  header: Authorization
  how_to_obtain: Create an API key in the DalalOS dashboard under API keys.
  location: header
  name: API key
  type: http-bearer
slug: dalalos-in-authentication
source_filename: dalalos-in-authentication.yml
source_heading: Authentication Profile
source_url: https://dalalos.in/docs/claude
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dalalos.in/docs/claude\nsources:\n- https://dalalos.in/docs/claude\n- https://dalalos.in/docs/cursor-and-other-ai-tools\n- https://dalalos.in/docs/rest-api\ndescription: Authentication methods for DalalOS\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Authorize once A sign-in window opens (Google or email code). Approve it, and Claude is connected. This sign-in standard is called\n    OAuth.\n- type: http-bearer\n  name: API key\n  evidence: 'Send an API key from your dashboard as Authorization: Bearer isk_live_… .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the DalalOS dashboard under API keys.\ndocs: https://dalalos.in/docs/claude\n"
source_yaml_url: https://artifacts.apis.io/dalalos-in/authentication/dalalos-in-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- Data
- Artificial Intelligence
- Stock Market
- MCP
---
