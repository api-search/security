---
anonymous_access: false
api_key_in: []
api_specs:
- filename: duve-openapi-generated.yml
  format: yaml
  label: Duve API
  slug: duve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duve/openapi/_ae-authored/duve-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Duve Authentication
name_suffix: Authentication
oauth_flows: []
overview: Duve declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Duve
provider_slug: duve
scheme_count: 1
schemes:
- evidence: Use this request to create a bearer token which will be used after for authenticating the rest of the requests in the OpenApi.
  flows:
  - client_credentials
  how_to_obtain: POST to the token endpoint with `client_id`, `client_secret`, and `grant_type=client_credentials` (optionally `scope`). The response contains an `access_token` (JWT) to be used as a Bearer token in the `Authorization` header of subsequent API calls.
  name: client_credentials
  token_url: https://sandbox.duve.com/api/openapi/v1/oauth2/token
  type: oauth2
slug: duve-authentication
source_filename: duve-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.duve.com/api-references/open-api/open-api/authorization/token.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.duve.com/api-references/open-api/open-api/authorization/token.md\nsources:\n- https://developers.duve.com/api-references/open-api/open-api/authorization/token.md\n- https://developers.duve.com/api-references/open-api/open-api/accounts/account-token.md\nschemes:\n- type: oauth2\n  name: client_credentials\n  evidence: Use this request to create a bearer token which will be used after for authenticating the rest of the requests in the OpenApi.\n  flows:\n  - client_credentials\n  token_url: https://sandbox.duve.com/api/openapi/v1/oauth2/token\n  how_to_obtain: POST to the token endpoint with `client_id`, `client_secret`, and `grant_type=client_credentials` (optionally `scope`). The response\n    contains an `access_token` (JWT) to be used as a Bearer token in the `Authorization` header of subsequent API calls.\ndocs: https://developers.duve.com/api-references/open-api/open-api/authorization/token.md\n"
source_yaml_url: https://artifacts.apis.io/duve/authentication/duve-authentication.yml
summary_line: 1 scheme
tags:
- Hospitality
- GuestExperience
- SaaS
- AI
- RevenueOptimization
- Company
---
