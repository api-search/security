---
anonymous_access: false
api_key_in: []
api_specs:
- filename: foundryims-com-storefront-api-openapi.yml
  format: yaml
  label: Foundry IMS Storefront API
  slug: foundryims-com-storefront-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundryims-com/openapi/foundryims-com-storefront-api-openapi.yml
auth_types: []
description: Authentication methods for Foundry IMS APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Foundry IMS Authentication
name_suffix: Authentication
oauth_flows: []
overview: Foundry IMS declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Foundry IMS
provider_slug: foundryims-com
scheme_count: 2
schemes:
- evidence: 'Every API request authenticates with a bearer token: Authorization: Bearer <key> .'
  header: Authorization
  location: header
  name: API Key
  type: http-bearer
- authorize_url: https://api.foundryims.com/api/v1/oauth/authorize
  evidence: The authorization-code flow a third-party app uses to receive a scoped Foundry access token — endpoints, parameters, errors, and what the token actually is.
  flows:
  - authorization_code
  how_to_obtain: Obtain a client_id and client_secret from Foundry after app registration; then follow the authorization‑code flow.
  name: OAuth Authorization Code
  scopes:
  - products.read
  - orders.read
  type: oauth2
slug: foundryims-com-authentication
source_filename: foundryims-com-authentication.yml
source_heading: Authentication Profile
source_url: https://foundryims.com/docs/authentication/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://foundryims.com/docs/authentication/\nsources:\n- https://foundryims.com/docs/authentication/\n- https://foundryims.com/docs/app-oauth/\n- https://foundryims.com/docs/app-oauth-example/\ndescription: Authentication methods for Foundry IMS APIs\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Every API request authenticates with a bearer token: Authorization: Bearer <key> .'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth Authorization Code\n  evidence: The authorization-code flow a third-party app uses to receive a scoped Foundry access token — endpoints, parameters, errors, and what\n    the token actually is.\n  flows:\n  - authorization_code\n  authorize_url: https://api.foundryims.com/api/v1/oauth/authorize\n  scopes:\n  - products.read\n  - orders.read\n  how_to_obtain: Obtain a client_id and client_secret from Foundry after app\
  \ registration; then follow the authorization‑code flow.\ndocs: https://foundryims.com/docs/authentication/\n"
source_yaml_url: https://artifacts.apis.io/foundryims-com/authentication/foundryims-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Inventory
- E-Commerce
- Software-as-a-Service
- Integration
---
