---
anonymous_access: false
api_key_in: []
api_specs:
- filename: notepad-page-agent-tokens-api-openapi.yml
  format: yaml
  label: notepad.page Agent Tokens API
  slug: notepad-page-agent-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notepad-page/openapi/notepad-page-agent-tokens-api-openapi.yml
- filename: notepad-page-discovery-api-openapi.yml
  format: yaml
  label: notepad.page Discovery API
  slug: notepad-page-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notepad-page/openapi/notepad-page-discovery-api-openapi.yml
- filename: notepad-page-memory-api-openapi.yml
  format: yaml
  label: notepad.page Memory API
  slug: notepad-page-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notepad-page/openapi/notepad-page-memory-api-openapi.yml
- filename: notepad-page-pages-api-openapi.yml
  format: yaml
  label: notepad.page Pages API
  slug: notepad-page-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notepad-page/openapi/notepad-page-pages-api-openapi.yml
- filename: notepad-page-safety-api-openapi.yml
  format: yaml
  label: notepad.page Safety API
  slug: notepad-page-safety-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notepad-page/openapi/notepad-page-safety-api-openapi.yml
- filename: notepad-page-sharing-api-openapi.yml
  format: yaml
  label: notepad.page Sharing API
  slug: notepad-page-sharing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notepad-page/openapi/notepad-page-sharing-api-openapi.yml
- filename: notepad-page-waitlist-api-openapi.yml
  format: yaml
  label: notepad.page Waitlist API
  slug: notepad-page-waitlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notepad-page/openapi/notepad-page-waitlist-api-openapi.yml
auth_types: []
description: Authentication for notepad.page uses OAuth 2.1 with PKCE and dynamic client registration for the MCP connector, and bearer tokens for agent tokens.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: notepad.page Authentication
name_suffix: Authentication
oauth_flows: []
overview: notepad.page declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: notepad.page
provider_slug: notepad-page
scheme_count: 2
schemes:
- evidence: OAuth 2.1 with PKCE and dynamic client registration.
  how_to_obtain: Sign‑in uses your email plus a 6‑digit code entered in the same sign‑in window.
  name: MCP OAuth
  type: oauth2
- evidence: Agent tokens are named, scoped, expiring REST credentials for scheduled jobs.
  how_to_obtain: Minted via the REST API by requesting an agent token and approving it on the notepad's account page.
  name: Agent token
  type: http-bearer
slug: notepad-page-authentication
source_filename: notepad-page-authentication.yml
source_heading: Authentication Profile
source_url: https://notepad.page/llms-full.txt
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://notepad.page/llms-full.txt\nsources:\n- https://notepad.page/llms-full.txt\n- https://notepad.page/quickstart\ndescription: Authentication for notepad.page uses OAuth 2.1 with PKCE and dynamic client registration for the MCP connector, and bearer tokens\n  for agent tokens.\nschemes:\n- type: oauth2\n  name: MCP OAuth\n  evidence: OAuth 2.1 with PKCE and dynamic client registration.\n  how_to_obtain: Sign‑in uses your email plus a 6‑digit code entered in the same sign‑in window.\n- type: http-bearer\n  name: Agent token\n  evidence: Agent tokens are named, scoped, expiring REST credentials for scheduled jobs.\n  how_to_obtain: Minted via the REST API by requesting an agent token and approving it on the notepad's account page.\ndocs: https://notepad.page/llms-full.txt\n"
source_yaml_url: https://artifacts.apis.io/notepad-page/authentication/notepad-page-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Visual-Page-Builder
- Privacy
- Free Tier
- Software-as-a-Service
---
