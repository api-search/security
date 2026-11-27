---
anonymous_access: false
api_key_in: []
api_specs:
- filename: helipod-io-container-openapi-generated.yml
  format: yaml
  label: Helipod Container API
  slug: container-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helipod-io/openapi/_ae-authored/helipod-io-container-openapi-generated.yml
- filename: helipod-io-core-openapi-generated.yml
  format: yaml
  label: Helipod core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helipod-io/openapi/_ae-authored/helipod-io-core-openapi-generated.yml
- filename: helipod-io-email-openapi-generated.yml
  format: yaml
  label: Helipod Email API
  slug: email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helipod-io/openapi/_ae-authored/helipod-io-email-openapi-generated.yml
- filename: helipod-io-vps-openapi-generated.yml
  format: yaml
  label: Helipod VPS API
  slug: vps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helipod-io/openapi/_ae-authored/helipod-io-vps-openapi-generated.yml
auth_types: []
description: Authentication methods for Helipod APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Helipod Authentication
name_suffix: Authentication
oauth_flows: []
overview: Helipod declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Helipod
provider_slug: helipod-io
scheme_count: 1
schemes:
- authorize_url: https://helipod.io/oauth/authorize
  evidence: It is standard OAuth 2.1 with PKCE, the same sign-in the AI tools use.
  header: Authorization
  how_to_obtain: Register an app in the dashboard (Settings → Developer apps) to get a Client ID (hoa_…) and optionally a Client secret (hel_ocs_…). Use the Authorization Code flow with PKCE to obtain an access token (hel_oat_…).
  location: header
  name: Helipod OAuth
  scopes:
  - containers
  - vps:read
  - spend
  token_url: https://api.helipod.io/oauth/token
  type: oauth2
slug: helipod-io-authentication
source_filename: helipod-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.helipod.io/docs/helipod/api-keys
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.helipod.io/docs/helipod/api-keys\nsources:\n- https://docs.helipod.io/docs/helipod/api-keys\n- https://docs.helipod.io/docs/helipod/oauth-apps\n- https://docs.helipod.io/docs/guides/api-keys-and-mcp\ndescription: Authentication methods for Helipod APIs\nschemes:\n- type: oauth2\n  name: Helipod OAuth\n  evidence: It is standard OAuth 2.1 with PKCE, the same sign-in the AI tools use.\n  location: header\n  header: Authorization\n  token_url: https://api.helipod.io/oauth/token\n  authorize_url: https://helipod.io/oauth/authorize\n  scopes:\n  - containers\n  - vps:read\n  - spend\n  how_to_obtain: Register an app in the dashboard (Settings → Developer apps) to get a Client ID (hoa_…) and optionally a Client secret (hel_ocs_…).\n    Use the Authorization Code flow with PKCE to obtain an access token (hel_oat_…).\ndocs: https://docs.helipod.io/docs/helipod/api-keys\nnote:\
  \ 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/helipod-io/authentication/helipod-io-authentication.yml
summary_line: 1 scheme
tags:
- Cloud
- Platform-as-a-Service
- Indonesia
- Hosting
- Developers
---
