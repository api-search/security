---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chargerdojo-com-openapi-generated.yml
  format: yaml
  label: ChargerDojo API
  slug: chargerdojo-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chargerdojo-com/openapi/_ae-authored/chargerdojo-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for ChargerDojo public API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ChargerDojo Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChargerDojo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ChargerDojo
provider_slug: chargerdojo-com
scheme_count: 1
schemes:
- evidence: A cdojo_... API key created in the app under Settings.
  header: Authorization
  how_to_obtain: Create the key in the ChargerDojo web app under Settings → Credentials.
  location: header
  name: apiKey
  type: http-bearer
slug: chargerdojo-com-authentication
source_filename: chargerdojo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.chargerdojo.com/guide/create-an-api-key.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.chargerdojo.com/guide/create-an-api-key.md\nsources:\n- https://docs.chargerdojo.com/guide/create-an-api-key.md\n- https://docs.chargerdojo.com/api-reference/connections/run-the-ocpi-credentials-handshake-for-an-owned-connection.md\n- https://docs.chargerdojo.com/api-reference/reports/issue-a-public-share-token-for-an-owned-report.md\n- https://docs.chargerdojo.com/api-reference/reports/revoke-the-public-share-token-of-an-owned-report.md\ndescription: Authentication schemes for ChargerDojo public API\nschemes:\n- type: http-bearer\n  name: apiKey\n  evidence: A cdojo_... API key created in the app under Settings.\n  location: header\n  header: Authorization\n  how_to_obtain: Create the key in the ChargerDojo web app under Settings → Credentials.\ndocs: https://docs.chargerdojo.com/guide/create-an-api-key.md\n"
source_yaml_url: https://artifacts.apis.io/chargerdojo-com/authentication/chargerdojo-com-authentication.yml
summary_line: 1 scheme
tags:
- Electric Vehicles
- OCPI
- Testing
- Simulator
- Charging
---
