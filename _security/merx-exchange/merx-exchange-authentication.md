---
anonymous_access: false
api_key_in: []
api_specs:
- filename: merx-exchange-payments-api-openapi.yml
  format: yaml
  label: MERX Payments API
  slug: merx-exchange-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merx-exchange/openapi/merx-exchange-payments-api-openapi.yml
- filename: merx-exchange-tron-api-openapi.yml
  format: yaml
  label: MERX TRON API
  slug: merx-exchange-tron-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merx-exchange/openapi/merx-exchange-tron-api-openapi.yml
auth_types: []
description: Authentication methods for Merx API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: MERX Authentication
name_suffix: Authentication
oauth_flows: []
overview: MERX declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MERX
provider_slug: merx-exchange
scheme_count: 2
schemes:
- evidence: 'The Merx API supports two authentication methods: API keys for programmatic access and JWT tokens for web sessions.'
  header: X-API-Key
  how_to_obtain: Create a new API key via POST /api/v1/keys (requires an existing API key). The secret key is returned once and cannot be retrieved again.
  location: header
  name: API Key
  type: apiKey
- evidence: Web sessions use Bearer JWT tokens obtained from the login flow. Pass the token in the Authorization header.
  header: Authorization
  how_to_obtain: Obtain a JWT token through the login flow (not detailed on the page).
  location: header
  name: JWT Bearer Token
  type: http-bearer
slug: merx-exchange-authentication
source_filename: merx-exchange-authentication.yml
source_heading: Authentication Profile
source_url: https://merx.exchange/docs/getting-started/authentication
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://merx.exchange/docs/getting-started/authentication\nsources:\n- https://merx.exchange/docs/getting-started/authentication\n- https://merx.exchange/docs/api/keys/create\n- https://merx.exchange/docs/api/keys/list\n- https://merx.exchange/docs/api/keys/revoke\ndescription: Authentication methods for Merx API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'The Merx API supports two authentication methods: API keys for programmatic access and JWT tokens for web sessions.'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a new API key via POST /api/v1/keys (requires an existing API key). The secret key is returned once and cannot be retrieved\n    again.\n- type: http-bearer\n  name: JWT Bearer Token\n  evidence: Web sessions use Bearer JWT tokens obtained from the login flow. Pass the token in the Authorization header.\n  location: header\n  header:\
  \ Authorization\n  how_to_obtain: Obtain a JWT token through the login flow (not detailed on the page).\nnote: No OAuth2 flows are documented for Merx.\ndocs: https://merx.exchange/docs/getting-started/authentication\n"
source_yaml_url: https://artifacts.apis.io/merx-exchange/authentication/merx-exchange-authentication.yml
summary_line: 2 schemes
tags:
- Energy
- Blockchain
- Payments
- Automation
- Artificial Intelligence
---
