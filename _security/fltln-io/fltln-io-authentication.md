---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fltln-io-openapi-generated.yml
  format: yaml
  label: Faultline API
  slug: fltln-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fltln-io/openapi/_ae-authored/fltln-io-openapi-generated.yml
auth_types: []
description: Faultline authentication uses workspace‑wide API keys.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Faultline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Faultline declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Faultline
provider_slug: fltln-io
scheme_count: 2
schemes:
- evidence: 'You can send it as X-API-Key: flt_... or Authorization: Bearer flt_... .'
  header: X-API-Key
  how_to_obtain: Create a workspace‑wide API key in Settings → API Keys (Pro plan and above).
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'You can send it as X-API-Key: flt_... or Authorization: Bearer flt_... .'
  header: Authorization
  how_to_obtain: Create a workspace‑wide API key in Settings → API Keys (Pro plan and above).
  location: header
  name: Authorization
  type: http-bearer
slug: fltln-io-authentication
source_filename: fltln-io-authentication.yml
source_heading: Authentication Profile
source_url: https://fltln.io/docs/mcp/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fltln.io/docs/mcp/\nsources:\n- https://fltln.io/docs/mcp/\n- https://fltln.io/docs/security/\n- https://fltln.io/docs/\n- https://fltln.io/docs/aws-iam-role/\ndescription: Faultline authentication uses workspace‑wide API keys.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'You can send it as X-API-Key: flt_... or Authorization: Bearer flt_... .'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a workspace‑wide API key in Settings → API Keys (Pro plan and above).\n- type: http-bearer\n  name: Authorization\n  evidence: 'You can send it as X-API-Key: flt_... or Authorization: Bearer flt_... .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a workspace‑wide API key in Settings → API Keys (Pro plan and above).\nnote: No OAuth2, JWT, HMAC, MTLS, or other authentication methods are documented.\ndocs: https://fltln.io/docs/mcp/\n"
source_yaml_url: https://artifacts.apis.io/fltln-io/authentication/fltln-io-authentication.yml
summary_line: 2 schemes
tags:
- Monitoring
- SRE Tools
- AIOps
---
