---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lunch-flow-openapi-generated.yml
  format: yaml
  label: Lunch Flow API
  slug: lunch-flow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lunch-flow/openapi/_ae-authored/lunch-flow-openapi-generated.yml
auth_types: []
description: Authentication methods for Lunch Flow Platform API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lunch Flow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lunch Flow declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lunch Flow
provider_slug: lunch-flow
scheme_count: 2
schemes:
- evidence: Send Body Exchange an authorization code for tokens, or refresh an expired access token.
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Obtain client_id and client_secret from your Lunch Flow app settings and use them in the token request body.
  name: OAuth2
  token_url: https://example.com/api/platform/oauth/token
  type: oauth2
- evidence: 'Authorization BasicAuth Authorization Basic <token> Management endpoints: use client_id as username and client_secret as password.'
  header: Authorization
  how_to_obtain: Use the client_id as the username and client_secret as the password for HTTP Basic authentication.
  location: header
  name: BasicAuth
  type: http-basic
slug: lunch-flow-authentication
source_filename: lunch-flow-authentication.yml
source_heading: Authentication Profile
source_url: https://www.lunchflow.app/docs/api/platform-api/oauthToken
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.lunchflow.app/docs/api/platform-api/oauthToken\nsources:\n- https://www.lunchflow.app/docs/api/platform-api/oauthToken\n- https://www.lunchflow.app/docs/api/platform-api/deleteUser\n- https://www.lunchflow.app/docs/guides/get-started/quickstart\ndescription: Authentication methods for Lunch Flow Platform API\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: Send Body Exchange an authorization code for tokens, or refresh an expired access token.\n  flows:\n  - authorization_code\n  - refresh_token\n  token_url: https://example.com/api/platform/oauth/token\n  how_to_obtain: Obtain client_id and client_secret from your Lunch Flow app settings and use them in the token request body.\n- type: http-basic\n  name: BasicAuth\n  evidence: 'Authorization BasicAuth Authorization Basic <token> Management endpoints: use client_id as username and client_secret as password.'\n\
  \  location: header\n  header: Authorization\n  how_to_obtain: Use the client_id as the username and client_secret as the password for HTTP Basic authentication.\ndocs: https://www.lunchflow.app/docs/api/platform-api/oauthToken\n"
source_yaml_url: https://artifacts.apis.io/lunch-flow/authentication/lunch-flow-authentication.yml
summary_line: 2 schemes
tags:
- Fintech
- API
- Banking
- Integration
- OpenAPI
- Developer
---
