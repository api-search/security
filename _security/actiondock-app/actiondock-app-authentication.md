---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Actiondock App Authentication
name_suffix: Authentication
oauth_flows: []
overview: actiondock-app declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: actiondock-app
provider_slug: actiondock-app
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: API key provided per workspace, sent as Bearer token in Authorization header.
  scheme: bearer
  type: http
slug: actiondock-app-authentication
source_filename: actiondock-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/actiondock-app-openapi.yml\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: API key provided per workspace, sent as Bearer token in Authorization header."
source_yaml_url: https://artifacts.apis.io/actiondock-app/authentication/actiondock-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API
- AI
- MCP
- Gateway
- Human-in-the-loop
---
