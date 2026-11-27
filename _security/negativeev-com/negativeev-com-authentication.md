---
anonymous_access: false
api_key_in: []
api_specs:
- filename: negativeev-com-a2a-api-openapi.yml
  format: yaml
  label: NegativeEV A2a API
  slug: negativeev-com-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/negativeev-com/openapi/negativeev-com-a2a-api-openapi.yml
- filename: negativeev-com-keys-api-openapi.yml
  format: yaml
  label: NegativeEV Keys API
  slug: negativeev-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/negativeev-com/openapi/negativeev-com-keys-api-openapi.yml
- filename: negativeev-com-mcp-api-openapi.yml
  format: yaml
  label: NegativeEV MCP API
  slug: negativeev-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/negativeev-com/openapi/negativeev-com-mcp-api-openapi.yml
- filename: negativeev-com-slate-api-openapi.yml
  format: yaml
  label: NegativeEV Slate API
  slug: negativeev-com-slate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/negativeev-com/openapi/negativeev-com-slate-api-openapi.yml
- filename: negativeev-com-usage-api-openapi.yml
  format: yaml
  label: NegativeEV Usage API
  slug: negativeev-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/negativeev-com/openapi/negativeev-com-usage-api-openapi.yml
auth_types: []
description: Authentication for NegativeEV
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: NegativeEV Authentication
name_suffix: Authentication
oauth_flows: []
overview: NegativeEV declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: NegativeEV
provider_slug: negativeev-com
scheme_count: 2
schemes:
- evidence: 'negativeev.com is the protected resource: it verifies Supabase‑issued JWTs sent as `Authorization: Bearer <access token>`.'
  header: Authorization
  how_to_obtain: Sign in with an email one‑time code at https://negativeev.com/ to receive a Supabase access token, or mint an agent key (prefix nev_) via POST https://negativeev.com/keys.
  location: header
  name: Bearer
  scopes:
  - openid
  - profile
  - email
  - offline_access
  type: http-bearer
- evidence: 'Use: send it as `Authorization: Bearer nev_…` on any request this document covers.'
  header: Authorization
  how_to_obtain: A signed‑in member can mint a key via POST https://negativeev.com/keys with a Supabase access token.
  location: header
  name: Agent key
  type: other
slug: negativeev-com-authentication
source_filename: negativeev-com-authentication.yml
source_heading: Authentication Profile
source_url: https://negativeev.com/auth.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://negativeev.com/auth.md\nsources:\n- https://negativeev.com/auth.md\ndescription: Authentication for NegativeEV\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'negativeev.com is the protected resource: it verifies Supabase‑issued JWTs sent as `Authorization: Bearer <access token>`.'\n  location: header\n  header: Authorization\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  how_to_obtain: Sign in with an email one‑time code at https://negativeev.com/ to receive a Supabase access token, or mint an agent key (prefix nev_)\n    via POST https://negativeev.com/keys.\n- type: other\n  name: Agent key\n  evidence: 'Use: send it as `Authorization: Bearer nev_…` on any request this document covers.'\n  location: header\n  header: Authorization\n  how_to_obtain: A signed‑in member can mint a key via POST https://negativeev.com/keys with a Supabase\
  \ access token.\nnote: OAuth2 flows supported are authorization_code and refresh_token as described in the Supabase discovery document; specific token and authorize\n  URLs are not listed on the page.\ndocs: https://negativeev.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/negativeev-com/authentication/negativeev-com-authentication.yml
summary_line: 2 schemes
tags:
- Sports Betting
- simulation analysis
- parlay calculator
- AI Agents
---
