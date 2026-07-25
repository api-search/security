---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Canada Life Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Canada Life secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Canada Life
provider_slug: canada-life
scheme_count: 2
schemes:
- authorization_code_note: The authorization endpoint is published with a literal "-NOT-SUPPORTED" suffix, so the interactive authorization-code flow is switched off by design. This is a server-to-server partner gateway.
  authorization_code_supported: false
  authorization_endpoint: https://api.canadalife.com/oauth2/v1/authorize-NOT-SUPPORTED
  bearer_usage: Access tokens are presented as HTTP bearer tokens. Every business path probed on this host returned 403 anonymously, so no operation-level security requirement can be observed.
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://api.canadalife.com
  jwks_confirmed: true
  jwks_keys: 1
  jwks_kid: api-gateway-1
  jwks_uri: https://api.canadalife.com/oauth2/v1/jwks
  name: canadalife-gateway-oauth2
  openIdConnectUrl: https://api.canadalife.com/.well-known/openid-configuration
  response_types_supported:
  - code
  - token
  revocation_endpoint: https://api.canadalife.com/oauth2/v1/revoke
  scopes_note: scopes_supported is published as an empty array. No OAuth scope vocabulary is exposed publicly on the gateway.
  scopes_supported: []
  source: well-known/canada-life-openid-configuration.json
  status: 200
  subject_types_supported: public
  surface: partner API gateway
  token_endpoint: https://api.canadalife.com/oauth2/v1/generate
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - client_secret_jwt
  type: openIdConnect
  userinfo_endpoint: https://api.canadalife.com/oauth2/v1/userinfo
- authorization_endpoint: https://my.canadalife.com/services/oauth2/authorize
  claims_supported_count: 24
  end_session_endpoint: https://my.canadalife.com/services/auth/idp/oidc/logout
  frontchannel_logout_supported: true
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://my.canadalife.com/services/oauth2/introspect
  issuer: https://my.canadalife.com
  jwks_uri: https://my.canadalife.com/id/keys
  name: canadalife-customer-portal-oidc
  openIdConnectUrl: https://my.canadalife.com/.well-known/openid-configuration
  registration_endpoint: https://my.canadalife.com/services/oauth2/register
  response_types_supported:
  - code
  - token
  - token id_token
  revocation_endpoint: https://my.canadalife.com/services/oauth2/revoke
  scopes_note: Salesforce Experience Cloud platform scopes, not Canada Life business scopes. See scopes/canada-life-scopes.yml for the full list and the caveat.
  scopes_supported_count: 36
  source: well-known/canada-life-my-openid-configuration.json
  status: 200
  surface: my.canadalife.com retail customer portal (Salesforce Experience Cloud)
  token_endpoint: https://my.canadalife.com/services/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
  userinfo_endpoint: https://my.canadalife.com/services/oauth2/userinfo
slug: canada-life-authentication
source_filename: canada-life-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://api.canadalife.com/.well-known/openid-configuration,\n  https://api.canadalife.com/oauth2/v1/jwks,\n  https://my.canadalife.com/.well-known/openid-configuration\nnote: >-\n  Derived from live OpenID Connect discovery documents rather than from an OpenAPI\n  specification — Canada Life publishes no OpenAPI, so there are no securitySchemes to\n  read. Everything below was fetched anonymously on 2026-07-25 and is recorded verbatim\n  from the published discovery metadata.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [clientCredentials, authorizationCode]\n  interactive_flow_supported_on_gateway: false\n  self_serve_onboarding: false\n  onboarding: >-\n    No public signup. Gateway client credentials are issued through a partner,\n    distributor or MGA relationship; there is no application form on any public page.\nschemes:\n- name: canadalife-gateway-oauth2\n  type: openIdConnect\n\
  \  surface: partner API gateway\n  issuer: https://api.canadalife.com\n  openIdConnectUrl: https://api.canadalife.com/.well-known/openid-configuration\n  source: well-known/canada-life-openid-configuration.json\n  status: 200\n  token_endpoint: https://api.canadalife.com/oauth2/v1/generate\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - client_secret_jwt\n  authorization_endpoint: https://api.canadalife.com/oauth2/v1/authorize-NOT-SUPPORTED\n  authorization_code_supported: false\n  authorization_code_note: >-\n    The authorization endpoint is published with a literal \"-NOT-SUPPORTED\" suffix, so\n    the interactive authorization-code flow is switched off by design. This is a\n    server-to-server partner gateway.\n  userinfo_endpoint: https://api.canadalife.com/oauth2/v1/userinfo\n  revocation_endpoint: https://api.canadalife.com/oauth2/v1/revoke\n  jwks_uri: https://api.canadalife.com/oauth2/v1/jwks\n  jwks_confirmed: true\n  jwks_keys:\
  \ 1\n  jwks_kid: api-gateway-1\n  id_token_signing_alg_values_supported: [RS256]\n  response_types_supported: [code, token]\n  subject_types_supported: public\n  scopes_supported: []\n  scopes_note: >-\n    scopes_supported is published as an empty array. No OAuth scope vocabulary is\n    exposed publicly on the gateway.\n  bearer_usage: >-\n    Access tokens are presented as HTTP bearer tokens. Every business path probed on\n    this host returned 403 anonymously, so no operation-level security requirement can\n    be observed.\n- name: canadalife-customer-portal-oidc\n  type: openIdConnect\n  surface: my.canadalife.com retail customer portal (Salesforce Experience Cloud)\n  issuer: https://my.canadalife.com\n  openIdConnectUrl: https://my.canadalife.com/.well-known/openid-configuration\n  source: well-known/canada-life-my-openid-configuration.json\n  status: 200\n  authorization_endpoint: https://my.canadalife.com/services/oauth2/authorize\n  token_endpoint: https://my.canadalife.com/services/oauth2/token\n\
  \  userinfo_endpoint: https://my.canadalife.com/services/oauth2/userinfo\n  introspection_endpoint: https://my.canadalife.com/services/oauth2/introspect\n  revocation_endpoint: https://my.canadalife.com/services/oauth2/revoke\n  registration_endpoint: https://my.canadalife.com/services/oauth2/register\n  end_session_endpoint: https://my.canadalife.com/services/auth/idp/oidc/logout\n  jwks_uri: https://my.canadalife.com/id/keys\n  id_token_signing_alg_values_supported: [RS256]\n  response_types_supported: [code, token, 'token id_token']\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  frontchannel_logout_supported: true\n  scopes_supported_count: 36\n  scopes_note: >-\n    Salesforce Experience Cloud platform scopes, not Canada Life business scopes. See\n    scopes/canada-life-scopes.yml for the full list and the caveat.\n  claims_supported_count: 24\ntransport_security:\n  tls: TLSv1.3 on www.canadalife.com\n  hsts: true\n\
  \  see: security/canada-life-domain-security.yml\nnon_api_channels:\n- name: ACORD XML for Life via CLIEDIS\n  auth: Out of band. Distributor/carrier trading-partner agreements administered through\n    CLIEDIS, not through an OAuth gateway.\n  see: conformance/canada-life-conformance.yml\ndocs: null\ndocs_note: >-\n  Canada Life publishes no authentication documentation page. The OIDC discovery\n  documents above are the only published description of the auth model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canada-life/refs/heads/main/authentication/canada-life-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Insurance
- Canada
- Life Insurance
- Health Insurance
- Employee Benefits
- Group Retirement
- Carrier
- ACORD
- Partner Gated
- No Public API
---
