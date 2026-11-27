---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eodly-io-api-openapi.json
  format: json
  label: Eodly API API
  slug: eodly-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eodly-io/openapi/_original/eodly-io-api-openapi.json
auth_types: []
description: Authentication schemes for Eodly API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Eodly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eodly declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Eodly
provider_slug: eodly-io
scheme_count: 2
schemes:
- evidence: Eodly uses long-lived, organization-scoped API keys. Every request to the API must include a key as a Bearer token.
  header: Authorization
  how_to_obtain: Sign in to Eodly as a founder or lead, open Settings → Developer, create an API key, copy the secret (eodly_sk_...).
  location: header
  name: Authorization
  scopes:
  - reports:read
  - team:read
  type: http-bearer
- evidence: 'The X-API-Key: eodly_sk_YOUR_KEY header is also accepted.'
  header: X-API-Key
  how_to_obtain: Sign in to Eodly as a founder or lead, open Settings → Developer, create an API key, copy the secret (eodly_sk_...).
  location: header
  name: X-API-Key
  scopes:
  - reports:read
  - team:read
  type: apiKey
slug: eodly-io-authentication
source_filename: eodly-io-authentication.yml
source_heading: Authentication Profile
source_url: https://eodly.io/developers#authentication
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://eodly.io/developers#authentication\nsources:\n- https://eodly.io/developers#authentication\n- https://eodly.io/auth.md\n- https://eodly.io/docs/mcp-server\n- https://eodly.io/docs/getting-started\ndescription: Authentication schemes for Eodly API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: Eodly uses long-lived, organization-scoped API keys. Every request to the API must include a key as a Bearer token.\n  location: header\n  header: Authorization\n  scopes:\n  - reports:read\n  - team:read\n  how_to_obtain: Sign in to Eodly as a founder or lead, open Settings → Developer, create an API key, copy the secret (eodly_sk_...).\n- type: apiKey\n  name: X-API-Key\n  evidence: 'The X-API-Key: eodly_sk_YOUR_KEY header is also accepted.'\n  location: header\n  header: X-API-Key\n  scopes:\n  - reports:read\n  - team:read\n  how_to_obtain: Sign in to Eodly as\
  \ a founder or lead, open Settings → Developer, create an API key, copy the secret (eodly_sk_...).\nnote: No OAuth flows are provided; authentication is solely via long-lived API keys used as Bearer tokens or X-API-Key header.\ndocs: https://eodly.io/developers#authentication\n"
source_yaml_url: https://artifacts.apis.io/eodly-io/authentication/eodly-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Productivity
- Remote Work
- Team Management
- Reporting
---
