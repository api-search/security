---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nocthost-openapi-generated.yml
  format: yaml
  label: NoctHost API
  slug: nocthost-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nocthost/openapi/_ae-authored/nocthost-openapi-generated.yml
auth_types: []
description: Authentication for NoctHost API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: NoctHost Authentication
name_suffix: Authentication
oauth_flows: []
overview: NoctHost declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: NoctHost
provider_slug: nocthost
scheme_count: 2
schemes:
- evidence: 'Send "Authorization: Bearer <accessToken>" on every request below.'
  header: Authorization
  how_to_obtain: Obtain a JWT by POST /auth/login (or /auth/register) which returns an "accessToken" field.
  location: header
  name: JWT access token
  type: http-bearer
- evidence: 'For scripts, create a non-expiring API key in the dashboard (Profile -> API keys) and send it the same way: "Authorization: Bearer nh_...".'
  header: Authorization
  how_to_obtain: Create a non‑expiring API key in the dashboard under Profile → API keys.
  location: header
  name: API key
  type: http-bearer
slug: nocthost-authentication
source_filename: nocthost-authentication.yml
source_heading: Authentication Profile
source_url: https://nocthost.com/docs/api
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nocthost.com/docs/api\nsources:\n- https://nocthost.com/docs/api\ndescription: Authentication for NoctHost API\nschemes:\n- type: http-bearer\n  name: JWT access token\n  evidence: 'Send \"Authorization: Bearer <accessToken>\" on every request below.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a JWT by POST /auth/login (or /auth/register) which returns an \"accessToken\" field.\n- type: http-bearer\n  name: API key\n  evidence: 'For scripts, create a non-expiring API key in the dashboard (Profile -> API keys) and send it the same way: \"Authorization: Bearer\n    nh_...\".'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a non‑expiring API key in the dashboard under Profile → API keys.\nnote: No OAuth2 flows, apiKey, http-basic, jwt, hmac, mtls, or other schemes are documented.\ndocs: https://nocthost.com/docs/api\n"
source_yaml_url: https://artifacts.apis.io/nocthost/authentication/nocthost-authentication.yml
summary_line: 2 schemes
tags:
- Company
- VPS
- Cloud
- Crypto Payments
- GPU
---
