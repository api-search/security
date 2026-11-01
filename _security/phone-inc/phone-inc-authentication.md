---
anonymous_access: false
api_key_in: []
api_specs:
- filename: phone-inc-openapi-generated.yml
  format: yaml
  label: Phone Inc API
  slug: phone-inc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phone-inc/openapi/_ae-authored/phone-inc-openapi-generated.yml
auth_types: []
description: Authentication schemes for Phone.inc API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Phone Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phone Inc declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Phone Inc
provider_slug: phone-inc
scheme_count: 2
schemes:
- evidence: 'Send the token on every request to `/api/v1/*`. We accept three methods, in priority order: **X-Api-Key header** (`recommended`): `X-Api-Key: phk_...` — explicit and unambiguous.'
  header: X-Api-Key
  how_to_obtain: Generate one in the dashboard at https://app.phone.inc/api_keys.
  location: header
  name: API Key (header)
  type: apiKey
- authorize_url: https://app.phone.inc/oauth/authorize
  evidence: 'We support a single grant type: **authorization code with PKCE**. It works for native apps, single-page apps, and traditional server-side web apps.'
  how_to_obtain: Register an OAuth client via dynamic client registration at https://app.phone.inc/oauth/register.
  name: Phone.inc OAuth
  scopes:
  - api
  token_url: https://app.phone.inc/oauth/token
  type: oauth2
slug: phone-inc-authentication
source_filename: phone-inc-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.phone.inc/api/authentication.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.phone.inc/api/authentication.md\nsources:\n- https://docs.phone.inc/api/authentication.md\n- https://docs.phone.inc/api/oauth.md\n- https://docs.phone.inc/api/authentication\n- https://docs.phone.inc/api/oauth\ndescription: Authentication schemes for Phone.inc API\nschemes:\n- type: apiKey\n  name: API Key (header)\n  evidence: 'Send the token on every request to `/api/v1/*`. We accept three methods, in priority order: **X-Api-Key header** (`recommended`):\n    `X-Api-Key: phk_...` — explicit and unambiguous.'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Generate one in the dashboard at https://app.phone.inc/api_keys.\n- type: oauth2\n  name: Phone.inc OAuth\n  evidence: 'We support a single grant type: **authorization code with PKCE**. It works for native apps, single-page apps, and traditional server-side\n    web apps.'\n  token_url: https://app.phone.inc/oauth/token\n\
  \  authorize_url: https://app.phone.inc/oauth/authorize\n  scopes:\n  - api\n  how_to_obtain: Register an OAuth client via dynamic client registration at https://app.phone.inc/oauth/register.\ndocs: https://docs.phone.inc/api/authentication.md\nnote: 2 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/phone-inc/authentication/phone-inc-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Communications
- Cloud
- Business
- API
---
