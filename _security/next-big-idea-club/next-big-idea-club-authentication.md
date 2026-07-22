---
api_key_in: []
api_specs:
- filename: next-big-idea-club-members-openapi.yml
  format: yaml
  label: Next Big Idea Club Members API
  slug: next-big-idea-club-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/next-big-idea-club/refs/heads/main/openapi/next-big-idea-club-members-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Next Big Idea Club Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- password
- refreshToken
overview: Next Big Idea Club secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, password, and refreshToken flow(s).
provider_name: Next Big Idea Club
provider_slug: next-big-idea-club
scheme_count: 2
schemes:
- authorization_endpoint: https://nextbigideaclub.com/oauth/authorize/
  end_session_endpoint: https://nextbigideaclub.com/oauth/destroy/
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - user_credentials
  - implicit
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://nextbigideaclub.com/oauth/introspection/
  issuer: https://nextbigideaclub.com
  jwks_uri: https://nextbigideaclub.com/.well-known/keys/
  name: oauth2
  response_types_supported:
  - code
  - id_token
  - token id_token
  - code id_token
  revocation_endpoint: https://nextbigideaclub.com/oauth/destroy/
  scopes:
  - openid
  - profile
  - email
  - basic
  software: WP OAuth Server
  sources:
  - well-known/next-big-idea-club-openid-configuration.json
  token_endpoint: https://nextbigideaclub.com/oauth/token/
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: oauth2
  userinfo_endpoint: https://nextbigideaclub.com/oauth/me/
- name: openIdConnect
  openIdConnectUrl: https://nextbigideaclub.com/.well-known/openid-configuration
  sources:
  - well-known/next-big-idea-club-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
slug: next-big-idea-club-authentication
source_filename: next-big-idea-club-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://nextbigideaclub.com/.well-known/openid-configuration\ndocs: https://nextbigideaclub.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials, implicit, password, refreshToken]\n  software: WP OAuth Server\nschemes:\n  - name: oauth2\n    type: oauth2\n    software: WP OAuth Server\n    issuer: https://nextbigideaclub.com\n    authorization_endpoint: https://nextbigideaclub.com/oauth/authorize/\n    token_endpoint: https://nextbigideaclub.com/oauth/token/\n    userinfo_endpoint: https://nextbigideaclub.com/oauth/me/\n    introspection_endpoint: https://nextbigideaclub.com/oauth/introspection/\n    revocation_endpoint: https://nextbigideaclub.com/oauth/destroy/\n    end_session_endpoint: https://nextbigideaclub.com/oauth/destroy/\n    jwks_uri: https://nextbigideaclub.com/.well-known/keys/\n    grant_types_supported: [authorization_code, client_credentials,\
  \ refresh_token, user_credentials, implicit]\n    response_types_supported: [code, id_token, token id_token, code id_token]\n    token_endpoint_auth_methods_supported: [client_secret_basic]\n    id_token_signing_alg_values_supported: [RS256]\n    scopes: [openid, profile, email, basic]\n    sources: [well-known/next-big-idea-club-openid-configuration.json]\n  - name: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://nextbigideaclub.com/.well-known/openid-configuration\n    subject_types_supported: [public]\n    sources: [well-known/next-big-idea-club-openid-configuration.json]\nnotes: >\n  The provider exposes a full OAuth 2.0 / OpenID Connect surface via the WP OAuth Server plugin,\n  used to authenticate members across the web experience and the iOS/Android apps. The bespoke\n  members/v1 REST API (openapi/) is protected by these tokens.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/next-big-idea-club/refs/heads/main/authentication/next-big-idea-club-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Books
- Media
- Subscription
- Nonfiction
- Podcast
- Education
- Membership
---
