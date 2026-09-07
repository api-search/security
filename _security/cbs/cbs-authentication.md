---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- token
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Cbs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: CBS (Paramount Global) secures its APIs with oauth2, openIdConnect, and token across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: CBS (Paramount Global)
provider_slug: cbs
scheme_count: 2
schemes:
- issuer: https://help.cbs.com
  name: CBS Help Center OIDC
  note: This is the stock Salesforce Experience Cloud / Salesforce Identity discovery document served from a CBS-controlled host. The 36 entries in scopes_supported (api, web, openid, refresh_token, offline_access, chatter_api, cdp_*, einstein_gpt_api, mcp_api, …) are Salesforce platform scopes, NOT a CBS product-API scope reference, which is why this repository carries no scopes/ artifact — publishing them as "CBS OAuth scopes" would misdescribe what CBS actually offers.
  observed:
    authorization_endpoint: https://help.cbs.com/services/oauth2/authorize
    dpop_signing_alg_values_supported:
    - RS256
    - RS384
    - RS512
    - ES256
    - ES384
    - ES512
    - EdDSA
    id_token_signing_alg_values_supported:
    - RS256
    introspection_endpoint: https://help.cbs.com/services/oauth2/introspect
    jwks_uri: https://help.cbs.com/id/keys
    registration_endpoint: https://help.cbs.com/services/oauth2/register
    response_types_supported:
    - code
    - token
    - token id_token
    revocation_endpoint: https://help.cbs.com/services/oauth2/revoke
    scopes_supported_count: 36
    token_endpoint: https://help.cbs.com/services/oauth2/token
    token_endpoint_auth_methods_supported:
    - client_secret_post
    - client_secret_basic
    - private_key_jwt
    userinfo_endpoint: https://help.cbs.com/services/oauth2/userinfo
  openIdConnectUrl: https://help.cbs.com/.well-known/openid-configuration
  sources:
  - well-known/cbs-openid-configuration.json
  type: openIdConnect
- confidence: low
  in: query
  name: CBS Sports Fantasy access token
  note: Reference data (sport list, player list) is served with no credential at all. League-scoped resources require a league_id and an access token that CBS issues only to a member of at least one CBS Sports fantasy league; there is no self-serve key page, no documented header or parameter name in any live CBS document, and no OAuth flow. The parameter name recorded here comes from CBS's own retired developer centre and from third-party clients, not from a live CBS page, and is marked as such.
  observed:
    anonymous_reads:
    - GET https://api.cbssports.com/fantasy/sports?version=3.0&response_format=json -> 200
    - GET https://api.cbssports.com/fantasy/players/list?version=3.0&response_format=json&sport=football -> 200
    gated_reads:
    - GET https://api.cbssports.com/fantasy/league/details?version=3.0&response_format=json -> 400 "Missing league_id"
    - GET https://api.cbssports.com/fantasy/league/teams?version=3.0&response_format=json -> 400 "Missing league_id"
  parameter_name: access_token
  sources:
  - probe
  type: token
slug: cbs-authentication
source_filename: cbs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://help.cbs.com/.well-known/openid-configuration (HTTP 200) plus live anonymous\n  probes of https://api.cbssports.com/fantasy on 2026-09-05. CBS publishes no OpenAPI,\n  so nothing here is derived from a security scheme block — every statement below is an\n  observed response or a fetched discovery document.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - token\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  spec_derived: false\n  note: >-\n    There is no published authentication reference for either CBS API surface. The only\n    machine-readable auth metadata CBS serves anywhere is the OIDC discovery document on\n    the Salesforce-hosted CBS Help Center, and that governs the help centre, not the\n    Fantasy API.\nschemes:\n- name: CBS Help Center OIDC\n  type: openIdConnect\n  issuer: https://help.cbs.com\n  openIdConnectUrl: https://help.cbs.com/.well-known/openid-configuration\n\
  \  sources:\n  - well-known/cbs-openid-configuration.json\n  observed:\n    authorization_endpoint: https://help.cbs.com/services/oauth2/authorize\n    token_endpoint: https://help.cbs.com/services/oauth2/token\n    userinfo_endpoint: https://help.cbs.com/services/oauth2/userinfo\n    revocation_endpoint: https://help.cbs.com/services/oauth2/revoke\n    introspection_endpoint: https://help.cbs.com/services/oauth2/introspect\n    registration_endpoint: https://help.cbs.com/services/oauth2/register\n    jwks_uri: https://help.cbs.com/id/keys\n    response_types_supported: [code, token, token id_token]\n    token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic, private_key_jwt]\n    id_token_signing_alg_values_supported: [RS256]\n    dpop_signing_alg_values_supported: [RS256, RS384, RS512, ES256, ES384, ES512, EdDSA]\n    scopes_supported_count: 36\n  note: >-\n    This is the stock Salesforce Experience Cloud / Salesforce Identity discovery document\n    served\
  \ from a CBS-controlled host. The 36 entries in scopes_supported (api, web,\n    openid, refresh_token, offline_access, chatter_api, cdp_*, einstein_gpt_api, mcp_api,\n    …) are Salesforce platform scopes, NOT a CBS product-API scope reference, which is why\n    this repository carries no scopes/ artifact — publishing them as \"CBS OAuth scopes\"\n    would misdescribe what CBS actually offers.\n- name: CBS Sports Fantasy access token\n  type: token\n  in: query\n  parameter_name: access_token\n  sources:\n  - probe\n  observed:\n    anonymous_reads:\n    - GET https://api.cbssports.com/fantasy/sports?version=3.0&response_format=json -> 200\n    - GET https://api.cbssports.com/fantasy/players/list?version=3.0&response_format=json&sport=football -> 200\n    gated_reads:\n    - GET https://api.cbssports.com/fantasy/league/details?version=3.0&response_format=json -> 400 \"Missing league_id\"\n    - GET https://api.cbssports.com/fantasy/league/teams?version=3.0&response_format=json -> 400\
  \ \"Missing league_id\"\n  note: >-\n    Reference data (sport list, player list) is served with no credential at all. League-scoped\n    resources require a league_id and an access token that CBS issues only to a member of at\n    least one CBS Sports fantasy league; there is no self-serve key page, no documented header\n    or parameter name in any live CBS document, and no OAuth flow. The parameter name recorded\n    here comes from CBS's own retired developer centre and from third-party clients, not from\n    a live CBS page, and is marked as such.\n  confidence: low\ndocs: null\ndocs_note: >-\n  The authentication reference lived at http://developer.cbssports.com/documentation/api/ and\n  that host no longer resolves (NXDOMAIN, checked 2026-09-05). The last capture is\n  http://web.archive.org/web/20200807214908/http://developer.cbssports.com/ — an archive, not a\n  live provider page, so it is not wired as a pointer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cbs/refs/heads/main/authentication/cbs-authentication.yml
summary_line: oauth2/openIdConnect/token · 2 schemes
tags:
- Broadcasting
- CBS News
- CBS Sports
- Entertainment
- Media
- News
- Paramount
- Streaming
- Television
- Fantasy Sports
- Syndication
- RSS
- Fortune 500
---
