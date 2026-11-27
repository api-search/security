---
anonymous_access: false
api_key_in: []
api_specs:
- filename: griffnode-com-api-openapi.yml
  format: yaml
  label: GriffNode API API
  slug: griffnode-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/griffnode-com/openapi/_original/griffnode-com-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GriffNode Authentication
name_suffix: Authentication
oauth_flows: []
overview: GriffNode declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GriffNode
provider_slug: griffnode-com
scheme_count: 1
schemes:
- evidence: 'Pass your key in the Authorization header using the Bearer scheme:'
  header: Authorization
  how_to_obtain: Keys are managed in your Dashboard; use the live key (sk_live_…) for production and the test key (sk_test_…) for development.
  location: header
  name: Bearer
  type: http-bearer
slug: griffnode-com-authentication
source_filename: griffnode-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.griffnode.com/authentication
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.griffnode.com/authentication\nsources:\n- https://docs.griffnode.com/authentication\n- https://docs.griffnode.com/quick-start\n- https://docs.griffnode.com/wallet-setup\n- https://docs.griffnode.com/webhooks-setup\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Pass your key in the Authorization header using the Bearer scheme:'\n  location: header\n  header: Authorization\n  how_to_obtain: Keys are managed in your Dashboard; use the live key (sk_live_…) for production and the test key (sk_test_…) for development.\nnote: No OAuth2, apiKey, or other authentication schemes are documented.\ndocs: https://docs.griffnode.com/authentication\n"
source_yaml_url: https://artifacts.apis.io/griffnode-com/authentication/griffnode-com-authentication.yml
summary_line: 1 scheme
tags:
- Cryptocurrency
- Payments
- Non-Custodial
- Merchants
- Gateways
---
