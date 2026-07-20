---
api_key_in: []
auth_types:
- oauth2
description: Libryo's partner API authenticates with OAuth 2.0 authorization-code grant. A partner application sends a Libryo user to the platform authorization endpoint, receives an authorization code on its registered redirect URI, then exchanges that code plus a client secret for an access token at the API token endpoint. Client credentials (client_id / client_secret) are issued by Libryo to partners; there is no public self-service registration. Captured from Libryo's own public OAuth integration guide and confirmed against the live token endpoint.
kind: authentication
layout: security
method: searched
name: Libryo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Libryo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Libryo
provider_slug: libryo
scheme_count: 1
schemes:
- authorizationUrl: https://my.libryo.com/oauth/authorize
  client_registration: Manual. client_id and client_secret are provided to the partner by Libryo; the redirect_uri must be pre-registered against the client.
  description: Three-legged OAuth 2.0. Step 1 redirect the user to the authorization endpoint with client_id, redirect_uri, response_type=code and a space-delimited scope list. Step 2 the user logs into Libryo and approves or rejects; Libryo redirects back with either ?code=<authorization-code> or ?error=access_denied. Step 3 POST the code to the token endpoint with grant_type=authorization_code, client_id, client_secret and redirect_uri.
  detail: scopes/libryo-scopes.yml
  flow: authorizationCode
  grant_types:
  - authorization_code
  name: libryoOAuth2
  pkce: not documented
  refresh_token: not documented in the public guide
  scopes:
  - view-legal-report
  - search-legislation
  - list-libryos
  sources:
  - https://github.com/libryo/libryo-api-oauth-docs
  tokenUrl: https://api.libryo.com/api/v1/oauth/token
  type: oauth2
slug: libryo-authentication
source_filename: libryo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/libryo/libryo-api-oauth-docs\ndocs: https://github.com/libryo/libryo-api-oauth-docs\ndescription: >-\n  Libryo's partner API authenticates with OAuth 2.0 authorization-code grant. A partner\n  application sends a Libryo user to the platform authorization endpoint, receives an\n  authorization code on its registered redirect URI, then exchanges that code plus a\n  client secret for an access token at the API token endpoint. Client credentials\n  (client_id / client_secret) are issued by Libryo to partners; there is no public\n  self-service registration. Captured from Libryo's own public OAuth integration guide\n  and confirmed against the live token endpoint.\nsummary:\n  types:\n  - oauth2\nschemes:\n- name: libryoOAuth2\n  type: oauth2\n  flow: authorizationCode\n  grant_types:\n  - authorization_code\n  authorizationUrl: https://my.libryo.com/oauth/authorize\n  tokenUrl: https://api.libryo.com/api/v1/oauth/token\n\
  \  scopes:\n  - view-legal-report\n  - search-legislation\n  - list-libryos\n  client_registration: >-\n    Manual. client_id and client_secret are provided to the partner by Libryo; the\n    redirect_uri must be pre-registered against the client.\n  pkce: not documented\n  refresh_token: not documented in the public guide\n  description: >-\n    Three-legged OAuth 2.0. Step 1 redirect the user to the authorization endpoint with\n    client_id, redirect_uri, response_type=code and a space-delimited scope list. Step 2\n    the user logs into Libryo and approves or rejects; Libryo redirects back with either\n    ?code=<authorization-code> or ?error=access_denied. Step 3 POST the code to the token\n    endpoint with grant_type=authorization_code, client_id, client_secret and redirect_uri.\n  sources:\n  - https://github.com/libryo/libryo-api-oauth-docs\n  detail: scopes/libryo-scopes.yml\nverification:\n  probed: '2026-07-19'\n  notes: >-\n    An unauthenticated POST to https://api.libryo.com/api/v1/oauth/token\
  \ returned HTTP 400\n    with an RFC 6749 JSON error body ({\"error\":\"invalid_request\", ...,\"hint\":\"Check the\n    `client_id` parameter\"}), confirming a live OAuth 2.0 token endpoint. GET\n    https://my.libryo.com/oauth/authorize with an unknown client returned HTTP 401. The\n    error envelope shape (\"hint\" alongside error/error_description) is that of\n    thephpleague/oauth2-server, the library behind Laravel Passport, consistent with the\n    PHP/Laravel stack visible across Libryo's public repositories.\ncaveats: >-\n  Note that *.libryo.com resolves via a wildcard DNS record to the platform load balancer,\n  so hostnames such as developer.libryo.com and docs.libryo.com answer HTTP 200 with the\n  application login page and are NOT developer surfaces. Only the two endpoints above are\n  documented API endpoints.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/libryo/refs/heads/main/authentication/libryo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Regulatory Compliance
- Legal Tech
- Environmental Health and Safety
- Governance Risk and Compliance
- Legal Registers
- Regulatory Change Management
- Sustainability
- OAuth
---
