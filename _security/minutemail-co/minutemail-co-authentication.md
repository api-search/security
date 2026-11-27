---
anonymous_access: false
api_key_in: []
api_specs:
- filename: minutemail-co-openapi-generated.yml
  format: yaml
  label: MinuteMail API
  slug: minutemail-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minutemail-co/openapi/_ae-authored/minutemail-co-openapi-generated.yml
auth_types: []
description: Authentication methods for MinuteMail API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MinuteMail Authentication
name_suffix: Authentication
oauth_flows: []
overview: MinuteMail declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MinuteMail
provider_slug: minutemail-co
scheme_count: 1
schemes:
- authorize_url: https://minutemail.co/idp/oauth/authorize
  evidence: The mock IDP implements the OAuth 2.0 authorization code flow , with optional PKCE ( S256 ) and OpenID Connect ID tokens.
  header: Authorization
  how_to_obtain: Create an OAuth client in the MinuteMail dashboard and use its client_id and client_secret.
  location: header
  name: OAuth 2.0 Authorization Code
  scopes:
  - openid
  - email
  - profile
  token_url: https://minutemail.co/idp/oauth/token
  type: oauth2
slug: minutemail-co-authentication
source_filename: minutemail-co-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.minutemail.co/user-interface/api-keys/
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.minutemail.co/user-interface/api-keys/\nsources:\n- https://docs.minutemail.co/user-interface/api-keys/\n- https://docs.minutemail.co/idp/oauth-flow/\n- https://docs.minutemail.co/user-interface/api-keys\n- https://docs.minutemail.co/api/getting-started/\ndescription: Authentication methods for MinuteMail API\nschemes:\n- type: oauth2\n  name: OAuth 2.0 Authorization Code\n  evidence: The mock IDP implements the OAuth 2.0 authorization code flow , with optional PKCE ( S256 ) and OpenID Connect ID tokens.\n  location: header\n  header: Authorization\n  token_url: https://minutemail.co/idp/oauth/token\n  authorize_url: https://minutemail.co/idp/oauth/authorize\n  scopes:\n  - openid\n  - email\n  - profile\n  how_to_obtain: Create an OAuth client in the MinuteMail dashboard and use its client_id and client_secret.\ndocs: https://docs.minutemail.co/user-interface/api-keys/\n\
  note: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/minutemail-co/authentication/minutemail-co-authentication.yml
summary_line: 1 scheme
tags:
- Email Testing
- Auth Testing
- Mock OAuth
- REST API
- SDK
- MCP Server
- Ephemeral Mailboxes
---
