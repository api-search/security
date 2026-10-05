---
anonymous_access: false
api_key_in: []
api_specs:
- filename: blazepizza-blazepizza-api-api-openapi.yml
  format: yaml
  label: Blazepizza Blazepizza API
  slug: blazepizza-blazepizza-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blazepizza/refs/heads/main/openapi/blazepizza-blazepizza-api-api-openapi.yml
- filename: blazepizza-cat-pic-api-openapi.yml
  format: yaml
  label: Blazepizza Cat Pic API
  slug: blazepizza-cat-pic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blazepizza/refs/heads/main/openapi/blazepizza-cat-pic-api-openapi.yml
- filename: blazepizza-foo-api-openapi.yml
  format: yaml
  label: Blazepizza Foo API
  slug: blazepizza-foo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blazepizza/refs/heads/main/openapi/blazepizza-foo-api-openapi.yml
- filename: blazepizza-http-api-openapi.yml
  format: yaml
  label: Blazepizza HTTP API
  slug: blazepizza-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blazepizza/refs/heads/main/openapi/blazepizza-http-api-openapi.yml
- filename: blazepizza-image-api-openapi.yml
  format: yaml
  label: Blazepizza Image API
  slug: blazepizza-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blazepizza/refs/heads/main/openapi/blazepizza-image-api-openapi.yml
auth_types: []
description: Thanx uses a password‑less OAuth2 flow.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Blazepizza Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blazepizza declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Blazepizza
provider_slug: blazepizza
scheme_count: 1
schemes:
- authorize_url: https://api.thanxsandbox.com/oauth/authorize
  evidence: This endpoint triggers the passwordless login flow.
  flows:
  - authorization_code
  how_to_obtain: Obtain a client_id from Thanx and use the /oauth/authorize endpoint to receive an authorization code, then exchange it for an access token at /oauth/token.
  name: Thanx Passwordless OAuth2
  scopes:
  - passwordless
  type: oauth2
slug: blazepizza-authentication
source_filename: blazepizza-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.thanx.com/consumer/best-practices/onboarding-authentication.md
source_yaml: "generated: '2026-09-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.thanx.com/consumer/best-practices/onboarding-authentication.md\nsources:\n- https://docs.thanx.com/consumer/best-practices/onboarding-authentication.md\n- https://docs.thanx.com/consumer/sso/acquire-auth-code.md\n- https://docs.thanx.com/consumer/sso/acquire-auth-code-cross-domain.md\n- https://docs.thanx.com/consumer/sso/acquire-access-token.md\ndescription: Thanx uses a password‑less OAuth2 flow.\nschemes:\n- type: oauth2\n  name: Thanx Passwordless OAuth2\n  evidence: This endpoint triggers the passwordless login flow.\n  flows:\n  - authorization_code\n  authorize_url: https://api.thanxsandbox.com/oauth/authorize\n  scopes:\n  - passwordless\n  how_to_obtain: Obtain a client_id from Thanx and use the /oauth/authorize endpoint to receive an authorization code, then exchange it for an\n    access token at /oauth/token.\nnote: The cross‑domain flow uses a separate\
  \ endpoint (/oauth/authorize-cross-domain) but follows the same OAuth2 passwordless scheme.\ndocs: https://docs.thanx.com/consumer/best-practices/onboarding-authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blazepizza/refs/heads/main/authentication/blazepizza-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Fast Casual
- Pizza
- Restaurant
- Franchise
---
