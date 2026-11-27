---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cross-deck-com-openapi-generated.yml
  format: yaml
  label: Crossdeck API
  slug: cross-deck-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cross-deck-com/openapi/_ae-authored/cross-deck-com-openapi-generated.yml
auth_types: []
description: Crossdeck authenticates API requests using either a standard HTTP Bearer token or a dedicated API‑Key header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Crossdeck Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crossdeck declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Crossdeck
provider_slug: cross-deck-com
scheme_count: 1
schemes:
- evidence: 'Authenticate every request with Authorization: Bearer <key> .'
  header: Authorization
  how_to_obtain: Obtain a publishable or secret key (cd_pub_… or cd_sk_…) from the Crossdeck dashboard.
  location: header
  name: Bearer
  type: http-bearer
slug: cross-deck-com-authentication
source_filename: cross-deck-com-authentication.yml
source_heading: Authentication Profile
source_url: https://cross-deck.com/docs/api-keys/
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cross-deck.com/docs/api-keys/\nsources:\n- https://cross-deck.com/docs/api-keys/\n- https://cross-deck.com/docs/api-keys/index.md\n- https://cross-deck.com/docs/identify-users/\n- https://cross-deck.com/docs/quickstart-web/\ndescription: Crossdeck authenticates API requests using either a standard HTTP Bearer token or a dedicated API‑Key header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authenticate every request with Authorization: Bearer <key> .'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a publishable or secret key (cd_pub_… or cd_sk_…) from the Crossdeck dashboard.\nnote: No OAuth2 flows are described on the referenced pages. 1 extracted row(s) were dropped because their quote was not on the page.\ndocs: https://cross-deck.com/docs/api-keys/\n"
source_yaml_url: https://artifacts.apis.io/cross-deck-com/authentication/cross-deck-com-authentication.yml
summary_line: 1 scheme
tags:
- SDK
- Monetization
- Analytics
- Error Tracking
- Subscription
---
