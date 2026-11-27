---
anonymous_access: false
api_key_in: []
api_specs:
- filename: forkmate-ai-openapi-generated.yml
  format: yaml
  label: Forkmate API
  slug: forkmate-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forkmate-ai/openapi/_ae-authored/forkmate-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for Forkmate as described on the Connect page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Forkmate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forkmate declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Forkmate
provider_slug: forkmate-ai
scheme_count: 1
schemes:
- evidence: Sign‑in Web apps (Claude, ChatGPT, Gemini, Grok, Perplexity) use OAuth 2.1 with PKCE.
  flows:
  - authorization_code
  how_to_obtain: The client opens a Forkmate sign‑in page once and stores the returned token; no client ID or secret is required.
  name: Forkmate OAuth
  type: oauth2
slug: forkmate-ai-authentication
source_filename: forkmate-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://forkmate.ai/connect/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://forkmate.ai/connect/\nsources:\n- https://forkmate.ai/connect/\ndescription: Authentication methods for Forkmate as described on the Connect page.\nschemes:\n- type: oauth2\n  name: Forkmate OAuth\n  evidence: Sign‑in Web apps (Claude, ChatGPT, Gemini, Grok, Perplexity) use OAuth 2.1 with PKCE.\n  flows:\n  - authorization_code\n  how_to_obtain: The client opens a Forkmate sign‑in page once and stores the returned token; no client ID or secret is required.\ndocs: https://forkmate.ai/connect/\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/forkmate-ai/authentication/forkmate-ai-authentication.yml
summary_line: 1 scheme
tags:
- Health
- Nutrition
- Artificial Intelligence
- Free
- Calorie Tracker
---
