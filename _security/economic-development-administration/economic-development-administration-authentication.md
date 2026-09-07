---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Economic Development Administration Authentication
name_suffix: Authentication
oauth_flows: []
overview: Economic Development Administration declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Economic Development Administration
provider_slug: economic-development-administration
scheme_count: 1
schemes:
- dpop_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  - EdDSA
  endpoints:
    authorization: https://sfgrants.eda.gov/services/oauth2/authorize
    end_session: https://sfgrants.eda.gov/services/auth/idp/oidc/logout
    introspection: https://sfgrants.eda.gov/services/oauth2/introspect
    jwks: https://sfgrants.eda.gov/id/keys
    registration: https://sfgrants.eda.gov/services/oauth2/register
    revocation: https://sfgrants.eda.gov/services/oauth2/revoke
    token: https://sfgrants.eda.gov/services/oauth2/token
    userinfo: https://sfgrants.eda.gov/services/oauth2/userinfo
  evidence:
  - fetched: '2026-09-06'
    status: 200
    url: https://sfgrants.eda.gov/.well-known/openid-configuration
  - fetched: '2026-09-06'
    status: 200
    url: https://sfgrants.eda.gov/id/keys
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  id: eda-grants-portal-oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://sfgrants.eda.gov
  name: OpenID Connect — EDA Grants Management Portal
  openIdConnectUrl: https://sfgrants.eda.gov/.well-known/openid-configuration
  pkce: not-declared-in-metadata
  response_types_supported:
  - code
  - token
  - token id_token
  scopes_ref: scopes/economic-development-administration-scopes.yml
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
slug: economic-development-administration-authentication
source_filename: economic-development-administration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: https://sfgrants.eda.gov/.well-known/openid-configuration\nownership_note: >-\n  sfgrants.eda.gov is EDA's own subdomain (DNS CNAMEs to Salesforce siteforce.com)\n  hosting the \"EDA Grants Management Portal\"; the OpenID Provider metadata is served\n  by that tenant under EDA's domain with issuer https://sfgrants.eda.gov, so it\n  describes EDA's grants portal sign-in and not a third-party product. It is the\n  Salesforce Experience Cloud platform's standard OIDC surface, not an EDA-authored\n  developer auth programme.\nsummary: >-\n  EDA publishes no developer API and no public authentication documentation. The only\n  authentication surface reachable anonymously on an EDA-controlled host is the OpenID\n  Connect / OAuth 2.0 provider on sfgrants.eda.gov, which authenticates grantees into\n  the EDA Grants Management Portal. Every data endpoint behind it (/services/data/vXX.0,\n  /services/oauth2/register, /services/oauth2/introspect)\
  \ returned 401 to an anonymous\n  client, so the portal API is customer-gated.\nschemes:\n  - id: eda-grants-portal-oidc\n    type: openIdConnect\n    name: OpenID Connect — EDA Grants Management Portal\n    openIdConnectUrl: https://sfgrants.eda.gov/.well-known/openid-configuration\n    issuer: https://sfgrants.eda.gov\n    endpoints:\n      authorization: https://sfgrants.eda.gov/services/oauth2/authorize\n      token: https://sfgrants.eda.gov/services/oauth2/token\n      userinfo: https://sfgrants.eda.gov/services/oauth2/userinfo\n      revocation: https://sfgrants.eda.gov/services/oauth2/revoke\n      introspection: https://sfgrants.eda.gov/services/oauth2/introspect\n      registration: https://sfgrants.eda.gov/services/oauth2/register\n      jwks: https://sfgrants.eda.gov/id/keys\n      end_session: https://sfgrants.eda.gov/services/auth/idp/oidc/logout\n    grant_types:\n      - authorization_code\n      - implicit\n      - refresh_token\n    response_types_supported:\n      - code\n\
  \      - token\n      - token id_token\n    token_endpoint_auth_methods_supported:\n      - client_secret_post\n      - client_secret_basic\n      - private_key_jwt\n    id_token_signing_alg_values_supported:\n      - RS256\n    dpop_signing_alg_values_supported:\n      - RS256\n      - RS384\n      - RS512\n      - ES256\n      - ES384\n      - ES512\n      - EdDSA\n    pkce: not-declared-in-metadata\n    scopes_ref: scopes/economic-development-administration-scopes.yml\n    evidence:\n      - url: https://sfgrants.eda.gov/.well-known/openid-configuration\n        status: 200\n        fetched: '2026-09-06'\n      - url: https://sfgrants.eda.gov/id/keys\n        status: 200\n        fetched: '2026-09-06'\ndynamic_client_registration:\n  declared: true\n  endpoint: https://sfgrants.eda.gov/services/oauth2/register\n  anonymous_registration: false\n  evidence:\n    - url: https://sfgrants.eda.gov/services/oauth2/register\n      status: 401\n      method: POST\n      fetched: '2026-09-06'\n\
  \      note: >-\n        Registration endpoint is advertised in the discovery document but rejects an\n        unauthenticated RFC 7591 registration request, so client onboarding is manual\n        and administered by EDA.\ngaps:\n  - No public API reference, no published auth guide, no key-issuance path for\n    developers outside the grantee population.\n  - The main web property (www.eda.gov) could not be read at all — Cloudflare managed\n    challenge returns 403 to non-browser clients — so any auth documentation published\n    there is unverified rather than absent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/economic-development-administration/refs/heads/main/authentication/economic-development-administration-authentication.yml
summary_line: 1 scheme
tags:
- Economic Development
- Federal-Government
- Grants
- Public Sector
- Regional Development
- Economic Data
---
