---
anonymous_access: false
api_key_in: []
api_specs:
- filename: amdahl-ai-api-openapi.json
  format: json
  label: Amdahl Platform API API
  slug: amdahl-platform-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amdahl-ai/openapi/_original/amdahl-ai-api-openapi.json
auth_types: []
description: Authentication methods for the Amdahl Platform API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Amdahl Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amdahl declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Amdahl
provider_slug: amdahl-ai
scheme_count: 2
schemes:
- evidence: 'Manual rotation OAuth 2.1 access token Authorization: Bearer <access_token> Third-party apps acting on behalf of a user Refresh token flow'
  header: Authorization
  how_to_obtain: Obtain via standard OAuth 2.1 authorization flow (refresh token flow) as described in the platform documentation.
  location: header
  name: OAuth 2.1 access token
  type: http-bearer
- evidence: 'Supabase JWT Authorization: Bearer <jwt> + X-Client-Slug: <slug> First-party web app only'
  header: Authorization
  how_to_obtain: Issued by Supabase when signing in to the Amdahl console; used for first‑party web apps.
  location: header
  name: Supabase JWT
  type: http-bearer
slug: amdahl-ai-authentication
source_filename: amdahl-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.amdahl.ai/authentication
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.amdahl.ai/authentication\nsources:\n- https://docs.amdahl.ai/authentication\n- https://docs.amdahl.ai/quickstart\n- https://docs.amdahl.ai/onboarding\n- https://docs.amdahl.ai/skills/amdahl-onboarding/SKILL\ndescription: Authentication methods for the Amdahl Platform API\nschemes:\n- type: http-bearer\n  name: OAuth 2.1 access token\n  evidence: 'Manual rotation OAuth 2.1 access token Authorization: Bearer <access_token> Third-party apps acting on behalf of a user Refresh token\n    flow'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain via standard OAuth 2.1 authorization flow (refresh token flow) as described in the platform documentation.\n- type: http-bearer\n  name: Supabase JWT\n  evidence: 'Supabase JWT Authorization: Bearer <jwt> + X-Client-Slug: <slug> First-party web app only'\n  location: header\n  header: Authorization\n  how_to_obtain:\
  \ Issued by Supabase when signing in to the Amdahl console; used for first‑party web apps.\nnote: All three credential types resolve to the same payload and are accepted on the same endpoint. The API key can also be sent as a Bearer token;\n  a Bearer value starting with the reserved `amdhl_` prefix is treated as an API key. 1 extracted row(s) were dropped because their quote was\n  not on the page.\ndocs: https://docs.amdahl.ai/authentication\n"
source_yaml_url: https://artifacts.apis.io/amdahl-ai/authentication/amdahl-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Marketing
- Automation
- GPT
- Plugins
---
