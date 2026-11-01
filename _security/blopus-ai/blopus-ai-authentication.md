---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Blopus API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Blopus Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: blopus-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: blopus-ai
provider_slug: blopus-ai
scheme_count: 1
schemes:
- evidence: Every request authenticates with a bearer token. No OAuth dance, no signed requests — just an API key in a header.
  header: Authorization
  how_to_obtain: Create keys in the dashboard.
  location: header
  name: Authorization
  type: apiKey
slug: blopus-ai-authentication
source_filename: blopus-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://blopus.ai/docs/authentication
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://blopus.ai/docs/authentication\nsources:\n- https://blopus.ai/docs/authentication\n- https://blopus.ai/docs/quickstart\ndescription: Authentication schemes for Blopus API\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: Every request authenticates with a bearer token. No OAuth dance, no signed requests — just an API key in a header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys in the dashboard.\nnote: No OAuth flows, bearer token is sent as an API key in the Authorization header.\ndocs: https://blopus.ai/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/blopus-ai/authentication/blopus-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Search
- API
- MCP
---
