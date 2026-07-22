---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Terralayr Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: terralayr secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: terralayr
provider_slug: terralayr
scheme_count: 2
schemes:
- issuer: https://www.trlyr.com/
  name: openIdConnect
  openIdConnectUrl: https://www.trlyr.com/.well-known/openid-configuration
  sources:
  - well-known/terralayr-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://www.trlyr.com/umbraco/delivery/api/v1/security/member/authorize
    flow: authorizationCode
    refreshUrl: https://www.trlyr.com/umbraco/delivery/api/v1/security/member/token
    scopes:
      offline_access: Issue a refresh token for offline access
      openid: OpenID Connect authentication
    tokenUrl: https://www.trlyr.com/umbraco/delivery/api/v1/security/member/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  id_token_signing_alg_values_supported:
  - RS256
  name: oauth2
  sources:
  - well-known/terralayr-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: terralayr-authentication
source_filename: terralayr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.trlyr.com/.well-known/openid-configuration\ndocs: https://www.trlyr.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256, plain]\n  note: >-\n    Discovery-document-derived member-authentication surface (Umbraco CMS Delivery\n    API). The LAYR flexibility product API is B2B/private and publishes no OpenAPI\n    or public auth documentation.\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://www.trlyr.com/.well-known/openid-configuration\n  issuer: https://www.trlyr.com/\n  sources: [well-known/terralayr-openid-configuration.json]\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.trlyr.com/umbraco/delivery/api/v1/security/member/authorize\n    tokenUrl: https://www.trlyr.com/umbraco/delivery/api/v1/security/member/token\n    refreshUrl: https://www.trlyr.com/umbraco/delivery/api/v1/security/member/token\n\
  \    scopes:\n      openid: OpenID Connect authentication\n      offline_access: Issue a refresh token for offline access\n  grant_types_supported: [authorization_code, refresh_token]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  id_token_signing_alg_values_supported: [RS256]\n  sources: [well-known/terralayr-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terralayr/refs/heads/main/authentication/terralayr-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Climate
- Energy
- Battery Energy Storage
- Grid Flexibility
- Renewable Energy
- Cleantech
- Energy Trading
---
