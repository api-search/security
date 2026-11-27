---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fast-io-openapi-generated.yml
  format: yaml
  label: Fastio API
  slug: fast-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fast-io/openapi/_ae-authored/fast-io-openapi-generated.yml
auth_types: []
description: Fastio supports multiple authentication methods as documented.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Fastio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fastio declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Fastio
provider_slug: fast-io
scheme_count: 3
schemes:
- authorize_url: https://go.fast.io/api/current/oauth/authorize
  evidence: Fastio implements OAuth 2.0 with PKCE (Proof Key for Code Exchange) for secure authorization without passing user credentials through the client application.
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Dynamic client registration via POST /current/oauth/register/ and then follow the PKCE authorization flow (GET /current/oauth/authorize/, POST /current/oauth/token/).
  name: OAuth 2.0 PKCE
  scopes:
  - user
  - org
  - workspace
  - all_orgs
  - all_workspaces
  - all_shares
  - all_sign_envelopes
  type: oauth2
- evidence: 'Long-lived tokens for service-to-service communication. Created via the API or the web UI. Used with the same Authorization: Bearer {api_key} header format as JWTs.'
  header: Authorization
  how_to_obtain: Create an API key via the API or Fastio web UI.
  location: header
  name: API Key
  type: http-bearer
- evidence: Send HTTP Basic Auth ( email:password ) to get a JWT.
  header: Authorization
  how_to_obtain: GET /current/user/auth/ with Basic Authorization header containing base64(email:password).
  location: header
  name: Basic Auth to JWT (deprecated)
  type: http-basic
slug: fast-io-authentication
source_filename: fast-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fast.io/oauth.html
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fast.io/oauth.html\nsources:\n- https://docs.fast.io/oauth.html\n- https://docs.fast.io/auth.html\n- https://docs.fast.io/signing.html\ndescription: Fastio supports multiple authentication methods as documented.\nschemes:\n- type: oauth2\n  name: OAuth 2.0 PKCE\n  evidence: Fastio implements OAuth 2.0 with PKCE (Proof Key for Code Exchange) for secure authorization without passing user credentials through\n    the client application.\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://go.fast.io/api/current/oauth/authorize\n  scopes:\n  - user\n  - org\n  - workspace\n  - all_orgs\n  - all_workspaces\n  - all_shares\n  - all_sign_envelopes\n  how_to_obtain: Dynamic client registration via POST /current/oauth/register/ and then follow the PKCE authorization flow (GET /current/oauth/authorize/,\n    POST /current/oauth/token/).\n- type: http-bearer\n\
  \  name: API Key\n  evidence: 'Long-lived tokens for service-to-service communication. Created via the API or the web UI. Used with the same Authorization: Bearer\n    {api_key} header format as JWTs.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key via the API or Fastio web UI.\n- type: http-basic\n  name: Basic Auth to JWT (deprecated)\n  evidence: Send HTTP Basic Auth ( email:password ) to get a JWT.\n  location: header\n  header: Authorization\n  how_to_obtain: GET /current/user/auth/ with Basic Authorization header containing base64(email:password).\ndocs: https://docs.fast.io/oauth.html\n"
source_yaml_url: https://artifacts.apis.io/fast-io/authentication/fast-io-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Cloud Storage
- Collaboration
- Enterprise
- Productivity
---
