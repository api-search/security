---
anonymous_access: false
api_key_in: []
api_specs:
- filename: genuinegood-online-api-pass-api-openapi.yml
  format: yaml
  label: Genuine Good News API pass API
  slug: genuinegood-online-api-pass-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genuinegood-online/openapi/genuinegood-online-api-pass-api-openapi.yml
- filename: genuinegood-online-grant-brief-api-openapi.yml
  format: yaml
  label: Genuine Good News grant brief API
  slug: genuinegood-online-grant-brief-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genuinegood-online/openapi/genuinegood-online-grant-brief-api-openapi.yml
- filename: genuinegood-online-grant-detail-api-openapi.yml
  format: yaml
  label: Genuine Good News grant detail API
  slug: genuinegood-online-grant-detail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genuinegood-online/openapi/genuinegood-online-grant-detail-api-openapi.yml
- filename: genuinegood-online-grant-matching-api-openapi.yml
  format: yaml
  label: Genuine Good News grant matching API
  slug: genuinegood-online-grant-matching-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genuinegood-online/openapi/genuinegood-online-grant-matching-api-openapi.yml
- filename: genuinegood-online-grant-preflight-api-openapi.yml
  format: yaml
  label: Genuine Good News grant preflight API
  slug: genuinegood-online-grant-preflight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genuinegood-online/openapi/genuinegood-online-grant-preflight-api-openapi.yml
- filename: genuinegood-online-grants-api-openapi.yml
  format: yaml
  label: Genuine Good News Grants API
  slug: genuinegood-online-grants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genuinegood-online/openapi/genuinegood-online-grants-api-openapi.yml
auth_types: []
description: Authentication for Genuine Good Grants API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Genuine Good News Authentication
name_suffix: Authentication
oauth_flows: []
overview: Genuine Good News declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Genuine Good News
provider_slug: genuinegood-online
scheme_count: 1
schemes:
- evidence: Your client creates the token locally and sends it only over HTTPS.
  header: Authorization
  how_to_obtain: The client generates a random token locally (e.g., using crypto.randomUUID() and random bytes) prefixed with "ggp_" and stores it securely.
  location: header
  name: Bearer Token
  type: http-bearer
slug: genuinegood-online-authentication
source_filename: genuinegood-online-authentication.yml
source_heading: Authentication Profile
source_url: https://genuinegood.online/grants/quickstart
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://genuinegood.online/grants/quickstart\nsources:\n- https://genuinegood.online/grants/quickstart\ndescription: Authentication for Genuine Good Grants API\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: Your client creates the token locally and sends it only over HTTPS.\n  location: header\n  header: Authorization\n  how_to_obtain: The client generates a random token locally (e.g., using crypto.randomUUID() and random bytes) prefixed with \"ggp_\" and stores\n    it securely.\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the page.\ndocs: https://genuinegood.online/grants/quickstart\n"
source_yaml_url: https://artifacts.apis.io/genuinegood-online/authentication/genuinegood-online-authentication.yml
summary_line: 1 scheme
tags:
- Newsletters
- Grants API
- News
- Community
- Non-Profit
---
