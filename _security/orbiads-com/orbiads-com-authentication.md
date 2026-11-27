---
anonymous_access: false
api_key_in: []
api_specs:
- filename: orbiads-com-openapi-generated.yml
  format: yaml
  label: OrbiAds API
  slug: orbiads-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orbiads-com/openapi/_ae-authored/orbiads-com-openapi-generated.yml
auth_types: []
description: Authentication uses Google OAuth 2.0 Device Flow.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: OrbiAds Authentication
name_suffix: Authentication
oauth_flows: []
overview: OrbiAds declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OrbiAds
provider_slug: orbiads-com
scheme_count: 1
schemes:
- authorize_url: https://orbiads.com/device
  evidence: A single Google sign-in gives you access to all of OrbiAds — CLI, MCP and Skills.
  flows:
  - device_code
  how_to_obtain: Sign in with your Google account via the CLI command `orbiads auth login`, which starts the Device Flow.
  name: Google OAuth 2.0
  type: oauth2
slug: orbiads-com-authentication
source_filename: orbiads-com-authentication.yml
source_heading: Authentication Profile
source_url: https://orbiads.com/docs/cli/auth
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://orbiads.com/docs/cli/auth\nsources:\n- https://orbiads.com/docs/cli/auth\n- https://orbiads.com/docs/mcp/quickstart\n- https://orbiads.com/docs/cli/quickstart\n- https://orbiads.com/docs/getting-started\ndescription: Authentication uses Google OAuth 2.0 Device Flow.\nschemes:\n- type: oauth2\n  name: Google OAuth 2.0\n  evidence: A single Google sign-in gives you access to all of OrbiAds — CLI, MCP and Skills.\n  flows:\n  - device_code\n  authorize_url: https://orbiads.com/device\n  how_to_obtain: Sign in with your Google account via the CLI command `orbiads auth login`, which starts the Device Flow.\ndocs: https://orbiads.com/docs/cli/auth\n"
source_yaml_url: https://artifacts.apis.io/orbiads-com/authentication/orbiads-com-authentication.yml
summary_line: 1 scheme
tags:
- Advertising
- MCP
- Google Ad Manager
- Artificial Intelligence
- Automation
---
