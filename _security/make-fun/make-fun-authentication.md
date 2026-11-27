---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: make-fun-admin-api-openapi.yml
  format: yaml
  label: EZO Labs Inc. Admin API
  slug: make-fun-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/make-fun/openapi/make-fun-admin-api-openapi.yml
- filename: make-fun-agent-api-openapi.yml
  format: yaml
  label: EZO Labs Inc. Agent API
  slug: make-fun-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/make-fun/openapi/make-fun-agent-api-openapi.yml
- filename: make-fun-agent-prompt-api-openapi.yml
  format: yaml
  label: EZO Labs Inc. Agent Prompt API
  slug: make-fun-agent-prompt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/make-fun/openapi/make-fun-agent-prompt-api-openapi.yml
- filename: make-fun-archive-api-openapi.yml
  format: yaml
  label: EZO Labs Inc. Archive API
  slug: make-fun-archive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/make-fun/openapi/make-fun-archive-api-openapi.yml
- filename: make-fun-claims-api-openapi.yml
  format: yaml
  label: EZO Labs Inc. Claims API
  slug: make-fun-claims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/make-fun/openapi/make-fun-claims-api-openapi.yml
- filename: make-fun-community-api-openapi.yml
  format: yaml
  label: EZO Labs Inc. Community API
  slug: make-fun-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/make-fun/openapi/make-fun-community-api-openapi.yml
- filename: make-fun-competitions-api-openapi.yml
  format: yaml
  label: EZO Labs Inc. Competitions API
  slug: make-fun-competitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/make-fun/openapi/make-fun-competitions-api-openapi.yml
- filename: make-fun-entries-api-openapi.yml
  format: yaml
  label: EZO Labs Inc. Entries API
  slug: make-fun-entries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/make-fun/openapi/make-fun-entries-api-openapi.yml
- filename: make-fun-export-api-openapi.yml
  format: yaml
  label: EZO Labs Inc. Export API
  slug: make-fun-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/make-fun/openapi/make-fun-export-api-openapi.yml
- filename: make-fun-sponsor-api-openapi.yml
  format: yaml
  label: EZO Labs Inc. Sponsor API
  slug: make-fun-sponsor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/make-fun/openapi/make-fun-sponsor-api-openapi.yml
- filename: make-fun-submissions-api-openapi.yml
  format: yaml
  label: EZO Labs Inc. Submissions API
  slug: make-fun-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/make-fun/openapi/make-fun-submissions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: EZO Labs Inc. Authentication
name_suffix: Authentication
oauth_flows: []
overview: EZO Labs Inc. secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: EZO Labs Inc.
provider_slug: make-fun
scheme_count: 2
schemes:
- description: A personal API key (POST /api/auth/solana/key, or a session's POST /api/auth/api-key/create). Refused by the admin routes and the session-only ones.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/make-fun-openapi.json
  type: apiKey
- description: 'A signed-in session: the cookie the web sign-in sets (better-auth.session_token, unprefixed, over plain http), or the same token as Authorization: Bearer.'
  in: cookie
  name: session
  parameter: __Secure-better-auth.session_token
  sources:
  - openapi/make-fun-openapi.json
  type: apiKey
slug: make-fun-authentication
source_filename: make-fun-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/make-fun-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: A personal API key (POST /api/auth/solana/key, or a session's POST /api/auth/api-key/create).\n    Refused by the admin routes and the session-only ones.\n  sources:\n  - openapi/make-fun-openapi.json\n- name: session\n  type: apiKey\n  in: cookie\n  parameter: __Secure-better-auth.session_token\n  description: 'A signed-in session: the cookie the web sign-in sets (better-auth.session_token,\n    unprefixed, over plain http), or the same token as Authorization: Bearer.'\n  sources:\n  - openapi/make-fun-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/make-fun/authentication/make-fun-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- AI Agents
- Bounties
- USDC
- Solana
---
