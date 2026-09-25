---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Aidentified Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aidentified declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Aidentified
provider_slug: aidentified
scheme_count: 2
schemes:
- applies_to: https://matching-api.aidentified.com
  assessment: 'This is a resource-owner-password exchange in all but name: the long-lived secret an integrator holds is the human account password, not a scoped, revocable API credential. There is no key rotation surface, no scoping, and no per-integration credential documented.'
  bearer_format: JWT
  evidence: https://github.com/aidentified-llc/matching-api-cli/blob/main/aidentified_matching_api/token_service.py
  header: 'Authorization: Bearer <token>'
  id: matching_api_bearer
  scheme: bearer
  token_acquisition:
    client_caching: The first-party CLI caches the token on local disk keyed by a CRC32 of the API base URL and reuses it until expires_in has elapsed.
    credential_env_vars:
    - AID_EMAIL
    - AID_PASSWORD
    endpoint: POST https://matching-api.aidentified.com/login
    request_body:
      email: account email address
      password: account password
    response_body:
      bearer_token: the JWT to present on subsequent calls
      expires_in: token lifetime in seconds
  type: http
- applies_to: https://mcp.aidentified.com/mcp
  assessment: 'Correct and modern: PKCE-only, RFC 9728 resource metadata, RFC 8414 server metadata, RFC 7591 dynamic registration, published JWKS. This is the strongest part of Aidentified''s public developer surface and it is entirely undocumented on their own site.'
  challenge_observed: '401 with WWW-Authenticate: Bearer resource_metadata="https://mcp.aidentified.com/.well-known/oauth-protected-resource/mcp"'
  dynamic_client_registration: https://login.aidentified.com/v1/oauth2/register
  evidence:
  - well-known/aidentified-login-oauth-authorization-server.json
  - well-known/aidentified-login-openid-configuration.json
  - well-known/aidentified-mcp-oauth-protected-resource.json
  flows:
    authorizationCode:
      authorizationUrl: https://app.aidentified.com/oauth/authorize
      refreshUrl: https://login.aidentified.com/v1/oauth2/token
      scopes:
        email: Email address claim
        full_access: Full access (advertised by the OIDC discovery document only)
        offline_access: Refresh-token issuance
        openid: OpenID Connect subject identifier
        phone: Phone number claim
        profile: Basic profile claims
      tokenUrl: https://login.aidentified.com/v1/oauth2/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: mcp_oauth2
  id_token_signing_alg: RS256
  issuer: https://login.aidentified.com
  jwks_uri: https://login.aidentified.com/.well-known/jwks.json
  pkce: S256
  pkce_required: true
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
  userinfo_endpoint: https://login.aidentified.com/v1/oauth2/userinfo
slug: aidentified-authentication
source_filename: aidentified-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: >-\n  Two first-party sources, both public: (1) Aidentified's own Apache-2.0 CLI source at\n  https://github.com/aidentified-llc/matching-api-cli (aidentified_matching_api/token_service.py and\n  constants.py), which is the published client for the bulk contact-matching API; (2) the RFC 8414 /\n  RFC 9728 / OIDC discovery documents probed live at login.aidentified.com and mcp.aidentified.com on\n  2026-09-14 and saved under well-known/.\ndocs: https://support.aidentified.com/hc/en-us/articles/52599228720532-How-can-I-get-an-API-key-token\nsummary: >-\n  Aidentified runs two distinct, unrelated authentication models. The bulk contact-matching REST API\n  uses a password-grant-shaped login that exchanges an account email and password for a bearer JWT.\n  The MCP server uses standards-compliant OAuth 2.1 with PKCE against a Stytch-backed authorization\n  server on login.aidentified.com. There is no API-key scheme: the help center's\
  \ answer to\n  \"How can I get an API key/token?\" is, verbatim, \"For all Aidentified API inquiries, please contact\n  your sales representative.\"\n\nschemes:\n\n  - id: matching_api_bearer\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    applies_to: https://matching-api.aidentified.com\n    header: 'Authorization: Bearer <token>'\n    token_acquisition:\n      endpoint: POST https://matching-api.aidentified.com/login\n      request_body:\n        email: account email address\n        password: account password\n      response_body:\n        bearer_token: the JWT to present on subsequent calls\n        expires_in: token lifetime in seconds\n      credential_env_vars:\n        - AID_EMAIL\n        - AID_PASSWORD\n      client_caching: >-\n        The first-party CLI caches the token on local disk keyed by a CRC32 of the API base URL and\n        reuses it until expires_in has elapsed.\n    evidence: https://github.com/aidentified-llc/matching-api-cli/blob/main/aidentified_matching_api/token_service.py\n\
  \    assessment: >-\n      This is a resource-owner-password exchange in all but name: the long-lived secret an integrator\n      holds is the human account password, not a scoped, revocable API credential. There is no key\n      rotation surface, no scoping, and no per-integration credential documented.\n\n  - id: mcp_oauth2\n    type: oauth2\n    applies_to: https://mcp.aidentified.com/mcp\n    flows:\n      authorizationCode:\n        authorizationUrl: https://app.aidentified.com/oauth/authorize\n        tokenUrl: https://login.aidentified.com/v1/oauth2/token\n        refreshUrl: https://login.aidentified.com/v1/oauth2/token\n        scopes:\n          openid: OpenID Connect subject identifier\n          profile: Basic profile claims\n          email: Email address claim\n          phone: Phone number claim\n          offline_access: Refresh-token issuance\n          full_access: Full access (advertised by the OIDC discovery document only)\n    pkce: S256\n    pkce_required: true\n\
  \    grant_types:\n      - authorization_code\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - none\n    dynamic_client_registration: https://login.aidentified.com/v1/oauth2/register\n    userinfo_endpoint: https://login.aidentified.com/v1/oauth2/userinfo\n    jwks_uri: https://login.aidentified.com/.well-known/jwks.json\n    id_token_signing_alg: RS256\n    issuer: https://login.aidentified.com\n    challenge_observed: >-\n      401 with WWW-Authenticate: Bearer resource_metadata=\"https://mcp.aidentified.com/.well-known/oauth-protected-resource/mcp\"\n    evidence:\n      - well-known/aidentified-login-oauth-authorization-server.json\n      - well-known/aidentified-login-openid-configuration.json\n      - well-known/aidentified-mcp-oauth-protected-resource.json\n    assessment: >-\n      Correct and modern: PKCE-only, RFC 9728 resource metadata, RFC 8414 server\
  \ metadata, RFC 7591\n      dynamic registration, published JWKS. This is the strongest part of Aidentified's public\n      developer surface and it is entirely undocumented on their own site.\n\nidentity_vendor:\n  name: Stytch\n  basis: >-\n    login.aidentified.com is a CNAME to substantial-fig-5730.customers.stytch.com, the JWKS x5c\n    certificate carries O=Stytch, and 404 bodies from that host link to stytch.com error docs. The\n    issuer and every endpoint are on aidentified.com, so the surface is Aidentified's.\n\ngaps:\n  - No API-key or scoped-credential scheme is documented for the REST API.\n  - No mTLS, no signed requests, no OpenID Connect on the REST API.\n  - >-\n    The MCP OAuth server advertises an empty scopes_supported array on the protected resource, so an\n    agent cannot tell from metadata what it is asking permission for.\n  - No public reference documents either scheme; both were reconstructed from first-party source code\n    and live discovery documents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidentified/refs/heads/main/authentication/aidentified-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data Enrichment
- Wealth Management
- Financial Services
- Relationship Intelligence
- Sales Intelligence
- Prospecting
- Contact Data
- Identity Resolution
- MCP
---
