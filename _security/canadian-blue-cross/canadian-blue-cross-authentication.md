---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Canadian Blue Cross Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Blue Cross Canada secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Blue Cross Canada
provider_slug: canadian-blue-cross
scheme_count: 2
schemes:
- claims:
  - aud
  - exp
  - iat
  - iss
  - sub
  code_challenge_methods:
  - plain
  - S256
  endpoints:
    authorization: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/authorize
    end_session: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/signout
    jwks: https://pac.bluecross.ca/.well-known/jwks
    revocation: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/revoke
    token: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/token
    userinfo: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/userinfo
  flows:
  - flow: authorizationCode
    response_modes:
    - form_post
    - fragment
    - query
    response_types:
    - code
    scopes:
    - openid
    - offline_access
  - flow: refreshToken
    scopes:
    - offline_access
  id_token_signing_alg:
  - RS256
  issuer: https://pac.bluecross.ca/
  name: pacific-blue-cross-member-oidc
  notes:
  - Backed by OpenIddict — the token endpoint returns OpenIddict error_uri values (https://documentation.openiddict.com/errors/ID2029) on an unauthenticated POST.
  - No dynamic client registration endpoint is advertised; client_id must be provisioned out of band, and no self-serve registration page is published.
  - Claims set is the bare JWT registered-claim minimum (no profile/email claims advertised).
  openIdConnectUrl: https://pac.bluecross.ca/.well-known/openid-configuration
  parameters:
    authorization_response_iss_parameter_supported: true
    claims_parameter_supported: false
    request_parameter_supported: false
    request_uri_parameter_supported: false
  revocation_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  sources:
  - well-known/canadian-blue-cross-pac-openid-configuration.json
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- name: rfc8414-authorization-server-metadata
  note: /.well-known/oauth-authorization-server returns the same document as the OIDC discovery endpoint (byte-identical), so it is recorded as one authorization server presented under both RFC 8414 and OIDC Discovery.
  sources:
  - well-known/canadian-blue-cross-pac-oauth-authorization-server.json
  type: oauth2
slug: canadian-blue-cross-authentication
source_filename: canadian-blue-cross-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://pac.bluecross.ca/.well-known/openid-configuration\ndocs: null\nscope: >-\n  Blue Cross Canada publishes no API authentication programme — no API keys, no client\n  registration, no partner OAuth onboarding. The one machine-readable authentication contract\n  live anywhere in the federation is the OpenID Connect / OAuth 2.0 authorization server that\n  Pacific Blue Cross (pac.bluecross.ca) serves for Umbraco Content Delivery API member sign-in.\n  It is captured here verbatim because it is real, anonymous, and machine-readable — but it\n  authenticates website members against a CMS, not a claims, benefits, or eligibility API.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken]\n  pkce: [S256, plain]\n  public_api_auth: none\n  human_login_only: true\nschemes:\n- name: pacific-blue-cross-member-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://pac.bluecross.ca/.well-known/openid-configuration\n\
  \  issuer: https://pac.bluecross.ca/\n  sources:\n  - well-known/canadian-blue-cross-pac-openid-configuration.json\n  endpoints:\n    authorization: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/authorize\n    token: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/token\n    userinfo: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/userinfo\n    end_session: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/signout\n    revocation: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/revoke\n    jwks: https://pac.bluecross.ca/.well-known/jwks\n  flows:\n  - flow: authorizationCode\n    response_types: [code]\n    response_modes: [form_post, fragment, query]\n    scopes: [openid, offline_access]\n  - flow: refreshToken\n    scopes: [offline_access]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  revocation_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_alg:\
  \ [RS256]\n  code_challenge_methods: [plain, S256]\n  subject_types: [public]\n  claims: [aud, exp, iat, iss, sub]\n  parameters:\n    claims_parameter_supported: false\n    request_parameter_supported: false\n    request_uri_parameter_supported: false\n    authorization_response_iss_parameter_supported: true\n  notes:\n  - Backed by OpenIddict — the token endpoint returns OpenIddict error_uri values\n    (https://documentation.openiddict.com/errors/ID2029) on an unauthenticated POST.\n  - No dynamic client registration endpoint is advertised; client_id must be provisioned\n    out of band, and no self-serve registration page is published.\n  - Claims set is the bare JWT registered-claim minimum (no profile/email claims advertised).\n- name: rfc8414-authorization-server-metadata\n  type: oauth2\n  sources:\n  - well-known/canadian-blue-cross-pac-oauth-authorization-server.json\n  note: >-\n    /.well-known/oauth-authorization-server returns the same document as the OIDC discovery\n   \
  \ endpoint (byte-identical), so it is recorded as one authorization server presented under\n    both RFC 8414 and OIDC Discovery.\nabsent:\n- api_keys\n- http_basic_api_auth\n- http_bearer_api_key\n- mutualTLS\n- client_credentials_flow\n- dynamic_client_registration\n- partner_developer_onboarding\nmember_plan_auth:\n- plan: Alberta Blue Cross\n  host: ab.bluecross.ca\n  model: web session login (member / plan sponsor / provider portals); Cloudflare bot protection\n  discovery: none\n- plan: Ontario / Quebec Blue Cross (Canassurance)\n  host: on.bluecross.ca\n  model: web session login\n  discovery: none\n- plan: Medavie Blue Cross\n  host: www.medaviebc.ca\n  model: web session login (member, plan sponsor, health-professional portals)\n  discovery: none\n- plan: Saskatchewan Blue Cross\n  host: www.sk.bluecross.ca\n  model: web session login\n  discovery: none\n- plan: Manitoba Blue Cross\n  host: www.mb.bluecross.ca\n  model: web session login\n  discovery: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canadian-blue-cross/refs/heads/main/authentication/canadian-blue-cross-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Insurance
- Canada
- Health Insurance
- Dental Benefits
- Travel Insurance
- Life Insurance
- Employee Benefits
- Group Benefits
- Claims
- Carrier
- Association
- No Public API
---
