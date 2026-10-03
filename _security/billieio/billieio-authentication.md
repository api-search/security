---
anonymous_access: false
api_key_in: []
auth_types: []
description: OAuth 2.0 client‑credentials flow with Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Billieio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Billieio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Billieio
provider_slug: billieio
scheme_count: 1
schemes:
- evidence: This API uses OAuth 2.0 for secure authentication.
  flows:
  - client_credentials
  how_to_obtain: 'Obtain a JWT access token by sending a POST request to the token endpoint with `grant_type=client_credentials`, `client_id` and `client_secret` in the request body. The returned `access_token` is then sent in the `Authorization: Bearer <token>` header on subsequent API calls.'
  name: OAuth2
  token_url: https://paella-sandbox.billie.io/api/v2/oauth/token
  type: oauth2
slug: billieio-authentication
source_filename: billieio-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.billie.io/reference/authentication.md
source_yaml: "generated: '2026-09-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.billie.io/reference/authentication.md\nsources:\n- https://docs.billie.io/reference/authentication.md\n- https://docs.billie.io/reference/oauth_token_create.md\n- https://docs.billie.io/reference/oauth_token_validate.md\n- https://docs.billie.io/reference/oauth_token_revoke.md\ndescription: OAuth 2.0 client‑credentials flow with Bearer token in the Authorization header.\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: This API uses OAuth 2.0 for secure authentication.\n  flows:\n  - client_credentials\n  token_url: https://paella-sandbox.billie.io/api/v2/oauth/token\n  how_to_obtain: 'Obtain a JWT access token by sending a POST request to the token endpoint with `grant_type=client_credentials`, `client_id`\n    and `client_secret` in the request body. The returned `access_token` is then sent in the `Authorization: Bearer <token>` header on subsequent\n    API\
  \ calls.'\nnote: The same token endpoint is also available on the production server at https://paella.billie.io/api/v2/oauth/token.\ndocs: https://docs.billie.io/reference/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billieio/refs/heads/main/authentication/billieio-authentication.yml
summary_line: 1 scheme
tags:
- Fintech
- Payments
- B2B
- Europe
---
