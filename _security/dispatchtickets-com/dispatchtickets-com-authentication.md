---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dispatchtickets-com-openapi-generated.yml
  format: yaml
  label: Dispatch Tickets API
  slug: dispatchtickets-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dispatchtickets-com/openapi/_ae-authored/dispatchtickets-com-openapi-generated.yml
auth_types: []
description: 'Dispatch Tickets supports three authentication methods: API keys for server‑side integrations, sessions for the admin dashboard, and portal tokens for customer‑facing UIs.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dispatch Tickets Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dispatch Tickets declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dispatch Tickets
provider_slug: dispatchtickets-com
scheme_count: 1
schemes:
- evidence: 'Pass the API key in the Authorization header as a Bearer token: API key authentication curl https://api.dispatchtickets.com/v1/brands \ -H "Authorization: Bearer sk_live_your_api_key"'
  header: Authorization
  how_to_obtain: Generate API keys from the admin dashboard under Settings → API Keys → Create Key or programmatically via the API.
  location: header
  name: API Key
  type: http-bearer
slug: dispatchtickets-com-authentication
source_filename: dispatchtickets-com-authentication.yml
source_heading: Authentication Profile
source_url: https://dispatchtickets.com/docs/authentication/
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dispatchtickets.com/docs/authentication/\nsources:\n- https://dispatchtickets.com/docs/authentication/\n- https://dispatchtickets.com/docs/quickstart/\n- https://dispatchtickets.com/docs/email-setup/\n- https://dispatchtickets.com/docs/multi-brand/\ndescription: 'Dispatch Tickets supports three authentication methods: API keys for server‑side integrations, sessions for the admin dashboard,\n  and portal tokens for customer‑facing UIs.'\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Pass the API key in the Authorization header as a Bearer token: API key authentication curl https://api.dispatchtickets.com/v1/brands\n    \\ -H \"Authorization: Bearer sk_live_your_api_key\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate API keys from the admin dashboard under Settings → API Keys → Create Key or programmatically via the API.\ndocs: https://dispatchtickets.com/docs/authentication/\n\
  note: 2 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/dispatchtickets-com/authentication/dispatchtickets-com-authentication.yml
summary_line: 1 scheme
tags:
- Ticketing
- Help Desk
- API-First
- Software-as-a-Service
- Multi-brand
---
