---
anonymous_access: false
api_key_in: []
auth_types: []
description: Breezeway uses JWT tokens obtained via a client‑credentials style POST to an auth endpoint. The access token is sent in the `Authorization` header prefixed with `JWT`.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Breezeway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Breezeway declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Breezeway
provider_slug: breezeway
scheme_count: 1
schemes:
- evidence: To authenticate requests to the various Breezeway platform APIs, the access token must be provided in the request header `Authorization` and *must include* the scheme `JWT` as a prefix to the access token.
  header: Authorization
  how_to_obtain: Obtain a client id and client secret from the Breezeway credentials page, then POST them as JSON to the token URL to receive a JWT access token.
  location: header
  name: JWT
  token_url: https://api.breezeway.io/public/auth/v1/
  type: http-bearer
slug: breezeway-authentication
source_filename: breezeway-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.breezeway.io/docs/authentication.md
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.breezeway.io/docs/authentication.md\nsources:\n- https://developer.breezeway.io/docs/authentication.md\n- https://developer.breezeway.io/docs/authentication\n- https://help.breezeway.io/en/articles/11426822-two-factor-authentication\n- https://developer.breezeway.io/docs/obtaining-credentials.md\ndescription: Breezeway uses JWT tokens obtained via a client‑credentials style POST to an auth endpoint. The access token is sent in the `Authorization`\n  header prefixed with `JWT`.\nschemes:\n- type: http-bearer\n  name: JWT\n  evidence: To authenticate requests to the various Breezeway platform APIs, the access token must be provided in the request header `Authorization`\n    and *must include* the scheme `JWT` as a prefix to the access token.\n  location: header\n  header: Authorization\n  token_url: https://api.breezeway.io/public/auth/v1/\n  how_to_obtain: Obtain\
  \ a client id and client secret from the Breezeway credentials page, then POST them as JSON to the token URL to receive\n    a JWT access token.\nnote: The documentation does not define standard OAuth2 flows, authorize URLs, or scopes; token acquisition is performed via a POST request with\n  client credentials.\ndocs: https://developer.breezeway.io/docs/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breezeway/refs/heads/main/authentication/breezeway-authentication.yml
summary_line: 1 scheme
tags:
- Property Management
- Software-as-a-Service
- Operations Automation
- Guest Experience
- Real Estate
---
