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
description: Fastio supports OAuth 2.0 (PKCE) with bearer tokens, API keys used as bearer tokens, and a deprecated HTTP Basic authentication that returns a JWT.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fast Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fastio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Fastio
provider_slug: fast-io
scheme_count: 2
schemes:
- authorize_url: https://go.fast.io/api/current/oauth/authorize
  evidence: Fastio implements OAuth 2.0 with PKCE (Proof Key for Code Exchange) for secure authorization without passing user credentials through the client application.
  flows:
  - authorization_code
  how_to_obtain: Register a client via dynamic client registration (POST /current/oauth/register/) and perform the PKCE authorization code flow (GET /current/oauth/authorize/, POST /current/oauth/token/).
  name: Fastio OAuth2 PKCE
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
  how_to_obtain: Create an API key through the Fastio web UI or API (POST /current/oauth/register/ or related endpoint).
  location: header
  name: Fastio API Key
  type: apiKey
slug: fast-io-authentication
source_filename: fast-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fast.io/oauth.html
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fast.io/oauth.html\nsources:\n- https://docs.fast.io/oauth.html\n- https://docs.fast.io/auth.html\n- https://docs.fast.io/signing.html\ndescription: Fastio supports OAuth 2.0 (PKCE) with bearer tokens, API keys used as bearer tokens, and a deprecated HTTP Basic authentication that\n  returns a JWT.\nschemes:\n- type: oauth2\n  name: Fastio OAuth2 PKCE\n  evidence: Fastio implements OAuth 2.0 with PKCE (Proof Key for Code Exchange) for secure authorization without passing user credentials through\n    the client application.\n  flows:\n  - authorization_code\n  authorize_url: https://go.fast.io/api/current/oauth/authorize\n  scopes:\n  - user\n  - org\n  - workspace\n  - all_orgs\n  - all_workspaces\n  - all_shares\n  - all_sign_envelopes\n  how_to_obtain: Register a client via dynamic client registration (POST /current/oauth/register/) and perform the PKCE authorization\
  \ code flow\n    (GET /current/oauth/authorize/, POST /current/oauth/token/).\n- type: apiKey\n  name: Fastio API Key\n  evidence: 'Long-lived tokens for service-to-service communication. Created via the API or the web UI. Used with the same Authorization: Bearer\n    {api_key} header format as JWTs.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key through the Fastio web UI or API (POST /current/oauth/register/ or related endpoint).\ndocs: https://docs.fast.io/oauth.html\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/fast-io/authentication/fast-io-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Collaboration
- Workspace
- Automation
- Fastio
---
