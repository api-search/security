---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Just Publish Authentication
name_suffix: Authentication
oauth_flows: []
overview: Just Publish declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Just Publish
provider_slug: justpublish-ai
scheme_count: 1
schemes:
- evidence: 'Authentication: OAuth 2.1 - Just Publish registers itself, so there is no client ID or client secret to fill in'
  header: Authorization
  how_to_obtain: The client opens a sign‑in window the first time and receives an access token bound to the endpoint.
  location: header
  name: OAuth 2.1
  type: http-bearer
slug: justpublish-ai-authentication
source_filename: justpublish-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://justpublish.ai/docs/mcp
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://justpublish.ai/docs/mcp\nsources:\n- https://justpublish.ai/docs/mcp\nschemes:\n- type: http-bearer\n  name: OAuth 2.1\n  evidence: 'Authentication: OAuth 2.1 - Just Publish registers itself, so there is no client ID or client secret to fill in'\n  location: header\n  header: Authorization\n  how_to_obtain: The client opens a sign‑in window the first time and receives an access token bound to the endpoint.\ndocs: https://justpublish.ai/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/justpublish-ai/authentication/justpublish-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Websites
- Hosting
- Software-as-a-Service
- Publishing
---
