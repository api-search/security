---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dynamic-signal-openapi-generated.yml
  format: yaml
  label: Dynamic Signal API
  slug: dynamic-signal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamic-signal/openapi/_ae-authored/dynamic-signal-openapi-generated.yml
auth_types: []
description: Firstup authentication uses OAuth 2.0 flows. All flows return an access token that must be sent in the HTTP Authorization header as a Bearer token.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Dynamic Signal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dynamic Signal declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Dynamic Signal
provider_slug: dynamic-signal
scheme_count: 4
schemes:
- evidence: When you don’t need to act on behalf of a user, you can use the Client Credentials grant to get an access token.
  flows:
  - clientCredentials
  how_to_obtain: Contact Firstup to get your clientID and clientSecret, then POST to the token endpoint with grant_type=client_credentials, client_id and client_secret.
  name: Client Credentials Grant
  token_url: https://auth.socialchorus.com/oauth/token
  type: oauth2
- authorize_url: https://auth.socialchorus.com/oauth/authorize
  evidence: This method is for applications that require user interaction, such as web or mobile apps where a user logs in and authorizes access.
  flows:
  - authorizationCode
  how_to_obtain: Redirect the user to the authorize URL, then exchange the returned code at the token endpoint with grant_type=authorization_code, client_id, client_secret, redirect_uri and code.
  name: Authorization Code Grant
  token_url: https://auth.socialchorus.com/oauth/token
  type: oauth2
- authorize_url: https://auth.socialchorus.com/oauth/authorize
  evidence: PKCE (Proof Key for Code Exchange) is an OAuth 2.0 extension that secures public clients, such as mobile apps and single-page applications (SPAs) that cannot securely store a client secret.
  flows:
  - authorizationCode
  how_to_obtain: Generate a code_verifier and code_challenge, build the authorization URL with code_challenge and code_challenge_method=S256, then exchange the returned code at the token endpoint with grant_type=authorization_code, client_id, redirect_uri, code and code_verifier.
  name: Authorization Code Grant with PKCE
  token_url: https://auth.socialchorus.com/oauth/token
  type: oauth2
- evidence: JWT (JSON Web Token) authentication allows your service to act on behalf of a specific user or system identity without user login.
  flows:
  - clientCredentials
  how_to_obtain: Create a signed JWT, POST it to the token endpoint with grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer, and receive an access token.
  name: JWT Bearer Token Grant
  token_url: https://auth.socialchorus.com/oauth/token
  type: oauth2
slug: dynamic-signal-authentication
source_filename: dynamic-signal-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.firstup.io/gettingstarted/supported-authentication-methods.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.firstup.io/gettingstarted/supported-authentication-methods.md\nsources:\n- https://developers.firstup.io/gettingstarted/supported-authentication-methods.md\n- https://developers.firstup.io/authorization/authenticationandauthorization.md\n- https://developers.firstup.io/authorization/authentication-methods.md\n- https://developers.firstup.io/authorization/auth-code-grant-pkce.md\ndescription: Firstup authentication uses OAuth 2.0 flows. All flows return an access token that must be sent in the HTTP Authorization header\n  as a Bearer token.\nschemes:\n- type: oauth2\n  name: Client Credentials Grant\n  evidence: When you don’t need to act on behalf of a user, you can use the Client Credentials grant to get an access token.\n  flows:\n  - clientCredentials\n  token_url: https://auth.socialchorus.com/oauth/token\n  how_to_obtain: Contact Firstup to get your clientID\
  \ and clientSecret, then POST to the token endpoint with grant_type=client_credentials, client_id\n    and client_secret.\n- type: oauth2\n  name: Authorization Code Grant\n  evidence: This method is for applications that require user interaction, such as web or mobile apps where a user logs in and authorizes access.\n  flows:\n  - authorizationCode\n  token_url: https://auth.socialchorus.com/oauth/token\n  authorize_url: https://auth.socialchorus.com/oauth/authorize\n  how_to_obtain: Redirect the user to the authorize URL, then exchange the returned code at the token endpoint with grant_type=authorization_code,\n    client_id, client_secret, redirect_uri and code.\n- type: oauth2\n  name: Authorization Code Grant with PKCE\n  evidence: PKCE (Proof Key for Code Exchange) is an OAuth 2.0 extension that secures public clients, such as mobile apps and single-page applications\n    (SPAs) that cannot securely store a client secret.\n  flows:\n  - authorizationCode\n  token_url: https://auth.socialchorus.com/oauth/token\n\
  \  authorize_url: https://auth.socialchorus.com/oauth/authorize\n  how_to_obtain: Generate a code_verifier and code_challenge, build the authorization URL with code_challenge and code_challenge_method=S256,\n    then exchange the returned code at the token endpoint with grant_type=authorization_code, client_id, redirect_uri, code and code_verifier.\n- type: oauth2\n  name: JWT Bearer Token Grant\n  evidence: JWT (JSON Web Token) authentication allows your service to act on behalf of a specific user or system identity without user login.\n  flows:\n  - clientCredentials\n  token_url: https://auth.socialchorus.com/oauth/token\n  how_to_obtain: Create a signed JWT, POST it to the token endpoint with grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer, and receive an\n    access token.\nnote: 'All flows require the access token to be sent as `Authorization: Bearer <access_token>`.'\ndocs: https://developers.firstup.io/gettingstarted/supported-authentication-methods.md\n"
source_yaml_url: https://artifacts.apis.io/dynamic-signal/authentication/dynamic-signal-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Employee Communication
- Enterprise Software
- SaaS
- HR Tech
---
