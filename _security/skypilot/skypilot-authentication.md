---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Skypilot Authentication
name_suffix: Authentication
oauth_flows: []
overview: SkyPilot declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: SkyPilot
provider_slug: skypilot
scheme_count: 2
schemes:
- evidence: 'Basic auth: Use an admin-configured username and password to authenticate.'
  header: Authorization
  how_to_obtain: Use an admin-configured username and password.
  location: header
  name: Basic auth
  type: http-basic
- evidence: 'To send a request to the service endpoint, a service client need to include the static API key in a request’s header:'
  header: Authorization
  how_to_obtain: Provide a static API key (e.g., AUTH_TOKEN) to the service and include it as a Bearer token in the Authorization header.
  location: header
  name: API key
  type: apiKey
slug: skypilot-authentication
source_filename: skypilot-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.skypilot.ai/en/latest/reference/auth.html.md
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.skypilot.ai/en/latest/reference/auth.html.md\nsources:\n- https://docs.skypilot.ai/en/latest/reference/auth.html.md\n- https://docs.skypilot.ai/en/latest/serving/auth.html.md\n- https://docs.skypilot.ai/en/latest/reference/auth.html\n- https://docs.skypilot.ai/en/latest/serving/auth.html\nschemes:\n- type: http-basic\n  name: Basic auth\n  evidence: 'Basic auth: Use an admin-configured username and password to authenticate.'\n  location: header\n  header: Authorization\n  how_to_obtain: Use an admin-configured username and password.\n- type: apiKey\n  name: API key\n  evidence: 'To send a request to the service endpoint, a service client need to include the static API key in a request’s header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Provide a static API key (e.g., AUTH_TOKEN) to the service and include it as a Bearer token in the Authorization\
  \ header.\ndocs: https://docs.skypilot.ai/en/latest/reference/auth.html.md\n"
source_yaml_url: https://artifacts.apis.io/skypilot/authentication/skypilot-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- OpenSource
- Compute
- Orchestration
---
