---
anonymous_access: false
api_key_in: []
auth_types: []
description: Laterbase authentication uses an API key provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Laterbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Laterbase declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Laterbase
provider_slug: laterbase-dev
scheme_count: 1
schemes:
- evidence: 'Antigravity takes serverUrl , not url , and the key goes in as written: it doesn''t read environment variables in headers.'
  header: Authorization
  how_to_obtain: Create an API key in the Connections dashboard; the key is shown once and must be copied into the configuration.
  location: header
  name: Laterbase API Key
  type: apiKey
slug: laterbase-dev-authentication
source_filename: laterbase-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://laterbase.dev/docs/connect/antigravity
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://laterbase.dev/docs/connect/antigravity\nsources:\n- https://laterbase.dev/docs/connect/antigravity\n- https://laterbase.dev/docs/connect/jetbrains\n- https://laterbase.dev/docs/connect/windsurf\n- https://laterbase.dev/docs/connect/cline\ndescription: Laterbase authentication uses an API key provided as a Bearer token in the Authorization header.\nschemes:\n- type: apiKey\n  name: Laterbase API Key\n  evidence: 'Antigravity takes serverUrl , not url , and the key goes in as written: it doesn''t read environment variables in headers.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the Connections dashboard; the key is shown once and must be copied into the configuration.\nnote: No OAuth2 or other authentication schemes are documented on the provided pages.\ndocs: https://laterbase.dev/docs/connect/antigravity\n"
source_yaml_url: https://artifacts.apis.io/laterbase-dev/authentication/laterbase-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Collaboration
- Productivity
- Automation
---
