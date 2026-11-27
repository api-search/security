---
anonymous_access: false
api_key_in: []
api_specs:
- filename: packetexchange-io-openapi-generated.yml
  format: yaml
  label: PacketExchange API
  slug: packetexchange-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/packetexchange-io/openapi/_ae-authored/packetexchange-io-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: PacketExchange Authentication
name_suffix: Authentication
oauth_flows: []
overview: PacketExchange declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PacketExchange
provider_slug: packetexchange-io
scheme_count: 1
schemes:
- evidence: 'Base URL: https://packetexchange.io/api/v1. Authenticate with `Authorization: Bearer <API key>`.'
  header: Authorization
  how_to_obtain: Create an API key via the dashboard or POST /api/v1/account/api-keys; the returned key is used as the Bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: packetexchange-io-authentication
source_filename: packetexchange-io-authentication.yml
source_heading: Authentication Profile
source_url: https://packetexchange.io/api-docs/reference/api-keys.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://packetexchange.io/api-docs/reference/api-keys.md\nsources:\n- https://packetexchange.io/api-docs/reference/api-keys.md\n- https://packetexchange.io/api-docs/reference/authentication\n- https://packetexchange.io/api-docs/reference/api-keys\n- https://packetexchange.io/api-docs/reference/switch-customer-trunks\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Base URL: https://packetexchange.io/api/v1. Authenticate with `Authorization: Bearer <API key>`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key via the dashboard or POST /api/v1/account/api-keys; the returned key is used as the Bearer token.\ndocs: https://packetexchange.io/api-docs/reference/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/packetexchange-io/authentication/packetexchange-io-authentication.yml
summary_line: 1 scheme
tags:
- Voice
- SMS
- VoIP
- Marketplace
---
