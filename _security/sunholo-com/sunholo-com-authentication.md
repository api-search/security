---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sunholo-com-openapi-generated.yml
  format: yaml
  label: Holosun ApS API
  slug: sunholo-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sunholo-com/openapi/_ae-authored/sunholo-com-openapi-generated.yml
auth_types: []
description: Authentication schemes as published on Sunholo documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Holosun ApS Authentication
name_suffix: Authentication
oauth_flows: []
overview: Holosun ApS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Holosun ApS
provider_slug: sunholo-com
scheme_count: 1
schemes:
- evidence: The sunholo.auth.oauth module provides a Google OAuth2 flow with token caching and credential refresh.
  how_to_obtain: Obtain a client_id and client_secret from Google and provide them to GoogleAuthManager.
  name: Google OAuth
  scopes:
  - openid
  - email
  - profile
  type: oauth2
slug: sunholo-com-authentication
source_filename: sunholo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://dev.sunholo.com/docs/auth/oauth/
source_yaml: "generated: '2026-11-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dev.sunholo.com/docs/auth/oauth/\nsources:\n- https://dev.sunholo.com/docs/auth/oauth/\n- https://dev.sunholo.com/docs/auth/\n- https://dev.sunholo.com/docs/config/\n- https://dev.sunholo.com/docs/auth/access-control/\ndescription: Authentication schemes as published on Sunholo documentation.\nschemes:\n- type: oauth2\n  name: Google OAuth\n  evidence: The sunholo.auth.oauth module provides a Google OAuth2 flow with token caching and credential refresh.\n  scopes:\n  - openid\n  - email\n  - profile\n  how_to_obtain: Obtain a client_id and client_secret from Google and provide them to GoogleAuthManager.\ndocs: https://dev.sunholo.com/docs/auth/oauth/\n"
source_yaml_url: https://artifacts.apis.io/sunholo-com/authentication/sunholo-com-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Platform
- Engineering
- Document-Processing
- Legal-Tech
---
