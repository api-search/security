---
anonymous_access: false
api_key_in: []
api_specs:
- filename: endurain-openapi-generated.yml
  format: yaml
  label: Endurain API
  slug: endurain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/endurain/openapi/_ae-authored/endurain-openapi-generated.yml
auth_types: []
description: Endurain supports API‑key authentication and OAuth 2.1 (including PKCE) flows.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Endurain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Endurain declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Endurain
provider_slug: endurain
scheme_count: 1
schemes:
- evidence: 'Send the raw key using either option: Option 1: X-API-Key header (recommended): POST /api/v1/activities/create/upload X-API-Key: endurain_abc12345...'
  header: X-API-Key
  how_to_obtain: Create an API key via the Endurain web UI (Settings → Security → API Keys) or the REST endpoint POST /api/v1/profile/api_keys (requires a JWT access token).
  location: header
  name: X-API-Key
  type: apiKey
slug: endurain-authentication
source_filename: endurain-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.endurain.com/reference/authentication/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.endurain.com/reference/authentication/\nsources:\n- https://docs.endurain.com/reference/authentication/\n- https://docs.endurain.com/integrate/authentication/\n- https://docs.endurain.com/integrate/api-keys/\n- https://docs.endurain.com/integrate/oauth-sso-pkce/\ndescription: Endurain supports API‑key authentication and OAuth 2.1 (including PKCE) flows.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Send the raw key using either option: Option 1: X-API-Key header (recommended): POST /api/v1/activities/create/upload X-API-Key:\n    endurain_abc12345...'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an API key via the Endurain web UI (Settings → Security → API Keys) or the REST endpoint POST /api/v1/profile/api_keys\n    (requires a JWT access token).\ndocs: https://docs.endurain.com/reference/authentication/\nnote: 1 extracted row(s) were\
  \ dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/endurain/authentication/endurain-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Fitness
- Self-hosted
- Open-source
- Privacy
---
