---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Madethis Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MadeThis secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MadeThis
provider_slug: madethis
scheme_count: 2
schemes:
- issuer: https://clerk.madethis.com
  name: MadeThisOIDC
  openIdConnectUrl: https://clerk.madethis.com/.well-known/openid-configuration
  sources:
  - well-known/madethis-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://clerk.madethis.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://clerk.madethis.com/oauth/token
    scope_count: 7
    tokenUrl: https://clerk.madethis.com/oauth/token
  name: MadeThisOAuth2
  sources:
  - well-known/madethis-oauth-authorization-server.json
  type: oauth2
slug: madethis-authentication
source_filename: madethis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://clerk.madethis.com/.well-known/openid-configuration\ndocs: https://clerk.com/docs/oauth/scoped-access\nscope_note: >-\n  MadeThis publishes no developer API and no API authentication documentation. The auth\n  profile below is NOT derived from an OpenAPI (there is none) — it is read verbatim from\n  the OIDC discovery and RFC 8414 metadata that MadeThis's own identity host,\n  clerk.madethis.com, serves anonymously. Those documents describe how a user (or an\n  OAuth client registered against MadeThis's Clerk instance) signs in to the MadeThis\n  product. They are not a contract for a public MadeThis API. Do not read this artifact\n  as evidence that MadeThis exposes callable endpoints.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  provider: Clerk (vendor-operated identity, MadeThis-controlled subdomain)\nschemes:\n- name: MadeThisOIDC\n  type: openIdConnect\n\
  \  openIdConnectUrl: https://clerk.madethis.com/.well-known/openid-configuration\n  issuer: https://clerk.madethis.com\n  sources: [well-known/madethis-openid-configuration.json]\n- name: MadeThisOAuth2\n  type: oauth2\n  sources: [well-known/madethis-oauth-authorization-server.json]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.madethis.com/oauth/authorize\n    tokenUrl: https://clerk.madethis.com/oauth/token\n    refreshUrl: https://clerk.madethis.com/oauth/token\n    scope_count: 7\nendpoints:\n  authorization: https://clerk.madethis.com/oauth/authorize\n  token: https://clerk.madethis.com/oauth/token\n  revocation: https://clerk.madethis.com/oauth/token/revoke\n  introspection: https://clerk.madethis.com/oauth/token_info\n  userinfo: https://clerk.madethis.com/oauth/userinfo\n  jwks: https://clerk.madethis.com/.well-known/jwks.json\ntoken:\n  id_token_signing_alg: [RS256]\n  client_auth_methods: [client_secret_basic, client_secret_post, none]\n  grant_types:\
  \ [authorization_code, refresh_token]\n  response_types: [code]\n  response_modes: [form_post, query]\n  code_challenge_methods: [S256]\n  subject_types: [public]\nclaims:\n- sub\n- iss\n- aud\n- exp\n- iat\n- email\n- email_verified\n- name\n- given_name\n- family_name\n- preferred_username\n- picture\n- org_id\nlogout:\n  backchannel_logout_supported: false\n  frontchannel_logout_supported: false\nx-evidence:\n- url: https://clerk.madethis.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n- url: https://clerk.madethis.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n- url: https://clerk.madethis.com/.well-known/jwks.json\n  http_status: 200\n  content_type: application/json\n- url: https://madethis.com/openapi.json\n  http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madethis/refs/heads/main/authentication/madethis-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Business Automation
- Software-as-a-Service
- Marketing Automation
- Startup Tools
- Y Combinator
- No-Code
- Website Builder
- E-Commerce
- Small Business
- AI Employees
---
