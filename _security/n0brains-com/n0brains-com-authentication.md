---
anonymous_access: false
api_key_in: []
api_specs:
- filename: n0brains-com-openapi-generated.yml
  format: yaml
  label: n0brains API
  slug: n0brains-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/n0brains-com/openapi/_ae-authored/n0brains-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: n0brains Authentication
name_suffix: Authentication
oauth_flows: []
overview: n0brains declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: n0brains
provider_slug: n0brains-com
scheme_count: 2
schemes:
- evidence: All authenticated endpoints require an API key via the X-API-Key header.
  header: X-API-Key
  how_to_obtain: Keys are generated on registration and can be rotated via POST /auth/api-keys.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'Login also returns a JWT token usable via Authorization: Bearer.'
  header: Authorization
  how_to_obtain: Obtained by logging in (or via the agent flow that returns a JWT token).
  location: header
  name: Bearer
  type: http-bearer
slug: n0brains-com-authentication
source_filename: n0brains-com-authentication.yml
source_heading: Authentication Profile
source_url: https://n0brains.com/docs/
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://n0brains.com/docs/\nsources:\n- https://n0brains.com/docs/\n- https://n0brains.com/docs/quickstart/\n- https://n0brains.com/es/docs/quickstart/\n- https://n0brains.com/tr/docs/quickstart/\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: All authenticated endpoints require an API key via the X-API-Key header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Keys are generated on registration and can be rotated via POST /auth/api-keys.\n- type: http-bearer\n  name: Bearer\n  evidence: 'Login also returns a JWT token usable via Authorization: Bearer.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtained by logging in (or via the agent flow that returns a JWT token).\nnote: OAuth flow details (token/authorize URLs) are not explicitly listed on the pages.\ndocs: https://n0brains.com/docs/\n"
source_yaml_url: https://artifacts.apis.io/n0brains-com/authentication/n0brains-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Trading
- Finance
- Market Data
- Pre-Trade
- Analytics
---
