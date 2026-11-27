---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mobiscroll-com-openapi-generated.yml
  format: yaml
  label: Mobiscroll API
  slug: mobiscroll-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobiscroll-com/openapi/_ae-authored/mobiscroll-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Mobiscroll APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mobiscroll Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mobiscroll declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Mobiscroll
provider_slug: mobiscroll-com
scheme_count: 2
schemes:
- authorize_url: /authorize
  evidence: 'Endpoint: GET /authorize'
  flows:
  - authorization_code
  how_to_obtain: Obtain client_id from the Mobiscroll Connect dashboard and use the /authorize endpoint to start the OAuth2 authorization code flow.
  name: OAuth2
  scopes:
  - free-busy
  - read
  - read-write
  type: oauth2
- evidence: The token works like a password — anyone who has it can install the Mobiscroll packages with your account.
  header: Authorization
  how_to_obtain: Generate a token via `mobiscroll login` and store it in the environment variable MOBISCROLL_NPM_TOKEN, referenced in .npmrc as //npm.mobiscroll.com/:_authToken = ${MOBISCROLL_NPM_TOKEN}.
  location: header
  name: NPM auth token
  type: http-bearer
slug: mobiscroll-com-authentication
source_filename: mobiscroll-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mobiscroll.com/docs/connect/api/oauth
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mobiscroll.com/docs/connect/api/oauth\nsources:\n- https://mobiscroll.com/docs/connect/api/oauth\n- https://mobiscroll.com/docs/javascript/guides/npm-auth-token\n- https://mobiscroll.com/docs/angular/guides/npm-auth-token\n- https://mobiscroll.com/docs/jquery/guides/npm-auth-token\ndescription: Authentication methods for Mobiscroll APIs\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: 'Endpoint: GET /authorize'\n  flows:\n  - authorization_code\n  authorize_url: /authorize\n  scopes:\n  - free-busy\n  - read\n  - read-write\n  how_to_obtain: Obtain client_id from the Mobiscroll Connect dashboard and use the /authorize endpoint to start the OAuth2 authorization code\n    flow.\n- type: http-bearer\n  name: NPM auth token\n  evidence: The token works like a password — anyone who has it can install the Mobiscroll packages with your account.\n  location: header\n  header:\
  \ Authorization\n  how_to_obtain: Generate a token via `mobiscroll login` and store it in the environment variable MOBISCROLL_NPM_TOKEN, referenced in .npmrc as\n    //npm.mobiscroll.com/:_authToken = ${MOBISCROLL_NPM_TOKEN}.\ndocs: https://mobiscroll.com/docs/connect/api/oauth\n"
source_yaml_url: https://artifacts.apis.io/mobiscroll-com/authentication/mobiscroll-com-authentication.yml
summary_line: 2 schemes
tags:
- UI
- Scheduling
- Calendar
- JavaScript
- OpenAPI
---
