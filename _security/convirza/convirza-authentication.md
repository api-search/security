---
anonymous_access: false
api_key_in: []
api_specs:
- filename: convirza-openapi-generated.yml
  format: yaml
  label: Convirza API
  slug: convirza-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/_ae-authored/convirza-openapi-generated.yml
auth_types: []
description: Convirza uses encrypted Bearer token authentication and OAuth 2.0 flows.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Convirza Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convirza declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Convirza
provider_slug: convirza
scheme_count: 1
schemes:
- evidence: Convirza uses **encrypted Bearer token authentication** with server-side session storage.
  header: Authorization
  how_to_obtain: Send your credentials to POST /oauth/token and receive an encrypted access_token and refresh_token.
  location: header
  name: Bearer Token
  token_url: /oauth/token
  type: http-bearer
slug: convirza-authentication
source_filename: convirza-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.convirza.com/authentication-2043390m0.md
source_yaml: "generated: '2026-10-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.convirza.com/authentication-2043390m0.md\nsources:\n- https://docs.convirza.com/authentication-2043390m0.md\n- https://docs.convirza.com/authentication-access-2395719m0.md\n- https://docs.convirza.com/working-with-encrypted-tokens-2043382m0.md\n- https://docs.convirza.com/get-access-token-32391152e0.md\ndescription: Convirza uses encrypted Bearer token authentication and OAuth 2.0 flows.\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: Convirza uses **encrypted Bearer token authentication** with server-side session storage.\n  location: header\n  header: Authorization\n  token_url: /oauth/token\n  how_to_obtain: Send your credentials to POST /oauth/token and receive an encrypted access_token and refresh_token.\ndocs: https://docs.convirza.com/authentication-2043390m0.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/authentication/convirza-authentication.yml
summary_line: 1 scheme
tags:
- Conversation Analytics
- Call Tracking
- AI
- Marketing
- Sales Enablement
---
