---
anonymous_access: false
api_key_in: []
api_specs:
- filename: requestly-openapi-generated.yml
  format: yaml
  label: Requestly API
  slug: requestly-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/requestly/openapi/_ae-authored/requestly-openapi-generated.yml
auth_types: []
description: Authentication methods supported by Requestly as documented
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Requestly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Requestly declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Requestly
provider_slug: requestly
scheme_count: 2
schemes:
- evidence: OAuth 1.0 is a signature‑based authorization scheme. Each request is signed with credentials you hold (a consumer key and access token, plus secrets) using a signature method you pick. The signature, signing parameters, and your credentials are sent in the `Authorization` header or in the request body.
  header: Authorization
  how_to_obtain: Provide Consumer Key, Consumer Secret, Access Token and Token Secret in the OAuth 1.0 fields; Requestly computes the signature and attaches it automatically.
  location: header or body
  name: OAuth 1.0
  type: other
- authorize_url: Provider's authorization endpoint (e.g. `https://provider.example.com/oauth/authorize`)
  evidence: 'OAuth 2.0 is the dominant authorization framework for modern APIs. Requestly handles the entire flow: it opens the provider''s consent screen when needed, exchanges the response for an access token, caches the token, refreshes it before it expires, and attaches it to every request.'
  flows:
  - authorization_code
  - authorization_code_pkce
  - client_credentials
  - implicit
  - password_credentials
  - manual_token
  header: Authorization
  how_to_obtain: Select a grant type, fill the required fields (Auth URL, Token URL, Client ID, Client Secret, etc.), and click **Get token**. Requestly runs the flow and stores the token.
  location: header
  name: OAuth 2.0
  token_url: Provider's token endpoint (e.g. `https://provider.example.com/oauth/token`)
  type: oauth2
slug: requestly-authentication
source_filename: requestly-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.requestly.com/api-client/send-api-request/authorization/oauth1.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.requestly.com/api-client/send-api-request/authorization/oauth1.md\nsources:\n- https://docs.requestly.com/api-client/send-api-request/authorization/oauth1.md\n- https://docs.requestly.com/api-client/send-api-request/authorization/oauth2.md\n- https://docs.requestly.com/api-client/git/providers-and-authentication.md\n- https://docs.requestly.com/api-client/send-api-request/authorization/digest.md\ndescription: Authentication methods supported by Requestly as documented\nschemes:\n- type: other\n  name: OAuth 1.0\n  evidence: OAuth 1.0 is a signature‑based authorization scheme. Each request is signed with credentials you hold (a consumer key and access token,\n    plus secrets) using a signature method you pick. The signature, signing parameters, and your credentials are sent in the `Authorization` header\n    or in the request body.\n  location: header or body\n  header:\
  \ Authorization\n  how_to_obtain: Provide Consumer Key, Consumer Secret, Access Token and Token Secret in the OAuth 1.0 fields; Requestly computes the signature\n    and attaches it automatically.\n- type: oauth2\n  name: OAuth 2.0\n  evidence: 'OAuth 2.0 is the dominant authorization framework for modern APIs. Requestly handles the entire flow: it opens the provider''s consent\n    screen when needed, exchanges the response for an access token, caches the token, refreshes it before it expires, and attaches it to every\n    request.'\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  - authorization_code_pkce\n  - client_credentials\n  - implicit\n  - password_credentials\n  - manual_token\n  token_url: Provider's token endpoint (e.g. `https://provider.example.com/oauth/token`)\n  authorize_url: Provider's authorization endpoint (e.g. `https://provider.example.com/oauth/authorize`)\n  how_to_obtain: Select a grant type, fill the required fields (Auth URL,\
  \ Token URL, Client ID, Client Secret, etc.), and click **Get token**.\n    Requestly runs the flow and stores the token.\ndocs: https://docs.requestly.com/api-client/send-api-request/authorization/oauth1.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/requestly/authentication/requestly-authentication.yml
summary_line: 2 schemes
tags:
- API
- Platform
- Testing
- Development
- Collaboration
- Security
---
