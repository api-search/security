---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tareno-co-openapi-generated.yml
  format: yaml
  label: Tareno API
  slug: tareno-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tareno-co/openapi/_ae-authored/tareno-co-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tareno Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tareno declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Tareno
provider_slug: tareno-co
scheme_count: 1
schemes:
- evidence: Choose OAuth, connect and sign in with your own Tareno account.
  header: Authorization
  how_to_obtain: Run the client‑specific login command (e.g., openclaw mcp login tareno or codex mcp login tareno) which opens a browser for Tareno OAuth sign‑in.
  location: header
  name: OAuth
  type: oauth2
slug: tareno-co-authentication
source_filename: tareno-co-authentication.yml
source_heading: Authentication Profile
source_url: https://tareno.co/docs/mcp
source_yaml: "generated: '2026-11-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tareno.co/docs/mcp\nsources:\n- https://tareno.co/docs/mcp\n- https://tareno.co/docs/plugins/openclaw\n- https://tareno.co/docs/plugins/hermes\n- https://tareno.co/docs/mcp/openai\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Choose OAuth, connect and sign in with your own Tareno account.\n  location: header\n  header: Authorization\n  how_to_obtain: Run the client‑specific login command (e.g., openclaw mcp login tareno or codex mcp login tareno) which opens a browser for Tareno\n    OAuth sign‑in.\ndocs: https://tareno.co/docs/mcp\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/tareno-co/authentication/tareno-co-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Social Media
- Automation
- Content Management
- SaaS
---
