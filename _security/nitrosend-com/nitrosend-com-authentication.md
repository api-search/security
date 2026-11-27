---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Nitrosend API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nitrosend Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nitrosend declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Nitrosend
provider_slug: nitrosend-com
scheme_count: 1
schemes:
- evidence: 'Pass your API key in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Generate an API key from Settings > API Keys in the dashboard; keys are prefixed with `nskey_live_` (or `wpkey_live_` for public website‑form keys).
  location: header
  name: BearerAuth
  type: http-bearer
slug: nitrosend-com-authentication
source_filename: nitrosend-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.nitrosend.com/authentication.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.nitrosend.com/authentication.md\nsources:\n- https://docs.nitrosend.com/authentication.md\n- https://docs.nitrosend.com/api/operations/operation-mcp-get.md\n- https://docs.nitrosend.com/api/operations/operation-v1-oauth-me-get.md\n- https://docs.nitrosend.com/api/operations/operation-v1-oauth-subscribe-post.md\ndescription: Authentication schemes for Nitrosend API\nschemes:\n- type: http-bearer\n  name: BearerAuth\n  evidence: 'Pass your API key in the `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key from Settings > API Keys in the dashboard; keys are prefixed with `nskey_live_` (or `wpkey_live_` for public\n    website‑form keys).\nnote: All authenticated endpoints accept the API key (or JWT/public key) as a Bearer token in the Authorization header. No OAuth2 flows are documented.\ndocs: https://docs.nitrosend.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/nitrosend-com/authentication/nitrosend-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Email
- Artificial Intelligence
- Marketing
- Automation
---
