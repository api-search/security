---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jev-agent-openapi-generated.yml
  format: yaml
  label: Jev Agent (Jagent) API
  slug: jev-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jev-agent/refs/heads/main/openapi/_ae-authored/jev-agent-openapi-generated.yml
auth_types: []
description: Jev API uses a bearer token sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Jev Agent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jev Agent (Jagent) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Jev Agent (Jagent)
provider_slug: jev-agent
scheme_count: 1
schemes:
- evidence: 'send it as Authorization: Bearer to api.typesafe.ai'
  header: Authorization
  how_to_obtain: Create a key in TypeSafe's console or obtain one from OpenRouter, Vercel, or the Jagent page after sign‑in.
  location: header
  name: Bearer
  type: http-bearer
slug: jev-agent-authentication
source_filename: jev-agent-authentication.yml
source_heading: Authentication Profile
source_url: https://jev-agent.com/playground
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://jev-agent.com/playground\nsources:\n- https://jev-agent.com/playground\n- https://jev-agent.com/api-access\n- https://jev-agent.com/getting-started\ndescription: Jev API uses a bearer token sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'send it as Authorization: Bearer to api.typesafe.ai'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in TypeSafe's console or obtain one from OpenRouter, Vercel, or the Jagent page after sign‑in.\ndocs: https://jev-agent.com/playground\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jev-agent/refs/heads/main/authentication/jev-agent-authentication.yml
summary_line: 1 scheme
tags:
- AI API
- Classification
- Token Billing
- Developer Tools
---
