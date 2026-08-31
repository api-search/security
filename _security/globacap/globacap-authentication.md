---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Globacap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Globacap declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Globacap
provider_slug: globacap
scheme_count: 1
schemes:
- authorization_endpoint: https://login.globacap.com/oauth2/auth
  claims_supported:
  - aud
  - exp
  - iat
  - iss
  - sub
  discovery_url: https://login.globacap.com/.well-known/openid-configuration
  end_session_endpoint: https://login.globacap.com/logout
  grant_types:
  - authorization_code
  - implicit
  - hybrid
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://login.globacap.com/oauth2/introspect
  jwks_uri: https://login.globacap.com/.well-known/jwks
  name: globacap-oidc
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  request_uri_parameter_supported: false
  response_modes_supported:
  - form_post
  - query
  - fragment
  response_types_supported:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - id_token token
  - code id_token token
  revocation_endpoint: https://login.globacap.com/oauth2/revoke
  scopes_supported:
  - address
  - email
  - offline
  - openid
  - phone
  - profile
  subject_types_supported:
  - public
  token_endpoint: https://login.globacap.com/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://login.globacap.com/oauth2/v2/user_profile
slug: globacap-authentication
source_filename: globacap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://login.globacap.com/.well-known/openid-configuration\nscope_of_this_artifact: >-\n  This describes the identity provider Globacap runs for its own platform\n  applications (investor.globacap.com, console.globacap.com). Globacap publishes no\n  public API reference and no machine-readable API contract, so there are no\n  documented API securitySchemes to derive from. Everything below is read verbatim\n  from the anonymous OpenID Connect discovery document served on Globacap's own\n  hostname; nothing is inferred.\nidentity_provider:\n  issuer: https://login.globacap.com\n  vendor: Kinde\n  vendor_evidence: login.globacap.com CNAMEs to eu.kinde.com\n  hostname_owned_by_provider: true\nschemes:\n- type: openIdConnect\n  name: globacap-oidc\n  discovery_url: https://login.globacap.com/.well-known/openid-configuration\n  jwks_uri: https://login.globacap.com/.well-known/jwks\n  authorization_endpoint: https://login.globacap.com/oauth2/auth\n\
  \  token_endpoint: https://login.globacap.com/oauth2/token\n  userinfo_endpoint: https://login.globacap.com/oauth2/v2/user_profile\n  revocation_endpoint: https://login.globacap.com/oauth2/revoke\n  introspection_endpoint: https://login.globacap.com/oauth2/introspect\n  end_session_endpoint: https://login.globacap.com/logout\n  grant_types:\n  - authorization_code\n  - implicit\n  - hybrid\n  response_types_supported:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - id_token token\n  - code id_token token\n  response_modes_supported:\n  - form_post\n  - query\n  - fragment\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n  id_token_signing_alg_values_supported:\n  - RS256\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  subject_types_supported:\n  - public\n  claims_supported:\n  - aud\n  - exp\n  - iat\n  - iss\n  - sub\n  scopes_supported:\n  - address\n  - email\n  - offline\n  - openid\n  - phone\n  - profile\n  request_uri_parameter_supported:\
  \ false\nedge_enforcement:\n- host: investor.globacap.com\n  mechanism: oauth2-proxy\n  evidence: 'Every path 302s to /oauth2/start?supports_reauth=true&rd=<path>; /api/* returns HTTP 401 with an empty JSON body.'\n- host: console.globacap.com\n  mechanism: oauth2-proxy\n  evidence: Every path 302s to /oauth2/start.\ngaps:\n- No public API authentication documentation exists; Globacap does not publish a developer portal or API reference.\n- Machine-to-machine / client_credentials support is not advertised in the discovery document.\n- No /.well-known/oauth-protected-resource (HTTP 404), so no RFC 9728 resource-server metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globacap/refs/heads/main/authentication/globacap-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Private Capital Markets
- Capital Markets
- Securities
- Financial-Services
- Fintech
- Tokenization
- Share Register
- Secondary Markets
- United Kingdom
---
