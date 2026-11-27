---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for hilos MCP API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: hilos Authentication
name_suffix: Authentication
oauth_flows: []
overview: hilos declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: hilos
provider_slug: hilos-sh
scheme_count: 1
schemes:
- evidence: 'Auth: an Authorization: Bearer <token> header on every request'
  header: Authorization
  how_to_obtain: In hilos, click an agent, choose Connect agent and Generate token. The token is shown once and can be copied.
  location: header
  name: Bearer token
  type: http-bearer
slug: hilos-sh-authentication
source_filename: hilos-sh-authentication.yml
source_heading: Authentication Profile
source_url: https://hilos.sh/docs/connect-your-agent
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hilos.sh/docs/connect-your-agent\nsources:\n- https://hilos.sh/docs/connect-your-agent\n- https://hilos.sh/docs/getting-started\ndescription: Authentication for hilos MCP API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Auth: an Authorization: Bearer <token> header on every request'\n  location: header\n  header: Authorization\n  how_to_obtain: In hilos, click an agent, choose Connect agent and Generate token. The token is shown once and can be copied.\ndocs: https://hilos.sh/docs/connect-your-agent\n"
source_yaml_url: https://artifacts.apis.io/hilos-sh/authentication/hilos-sh-authentication.yml
summary_line: 1 scheme
tags:
- Collaboration
- Artificial Intelligence
- Chat
- Developer Tools
- Productivity
---
