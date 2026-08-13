---
api_key_in: []
auth_types: []
description: eSentire publishes no OpenAPI and no developer authentication page, so this profile is built entirely from the two OAuth discovery documents the API host serves anonymously plus the challenge headers the gateway returns. It is therefore complete and accurate for the authorization layer, and silent on anything the docs would normally add (token lifetimes, key rotation, service accounts, IP allow-listing).
kind: authentication
layout: security
method: probed
name: Esentire Authentication
name_suffix: Authentication
oauth_flows: []
overview: eSentire declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: eSentire
provider_slug: esentire
scheme_count: 1
schemes:
- applies_to:
  - https://api.esentire.com/mcp
  flows:
    authorizationCode:
      authorizationUrl: https://esentire.okta.com/oauth2/v1/authorize
      refreshUrl: null
      scopes:
        email: End-user email claim
        openid: OpenID Connect subject identifier
        profile: End-user profile claims
      tokenUrl: https://esentire.okta.com/oauth2/v1/token
  format: Bearer <access_token>
  header: Authorization
  id: oauth2_okta
  identity_provider: Okta
  in: header
  issuer: https://esentire.okta.com
  note: The only grant type advertised is authorization_code. There is no client_credentials flow in the metadata, which means machine-to-machine access to this surface is not offered through the discovered authorization server — every token is issued against a human Okta identity.
  pkce:
    methods:
    - S256
    required: true
  type: oauth2
slug: esentire-authentication
source_filename: esentire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://api.esentire.com/.well-known/oauth-authorization-server\ndocs: null\nname: eSentire authentication profile\ndescription: >-\n  eSentire publishes no OpenAPI and no developer authentication page, so this\n  profile is built entirely from the two OAuth discovery documents the API host\n  serves anonymously plus the challenge headers the gateway returns. It is\n  therefore complete and accurate for the authorization layer, and silent on\n  anything the docs would normally add (token lifetimes, key rotation, service\n  accounts, IP allow-listing).\nschemes:\n- id: oauth2_okta\n  type: oauth2\n  in: header\n  header: Authorization\n  format: Bearer <access_token>\n  flows:\n    authorizationCode:\n      authorizationUrl: https://esentire.okta.com/oauth2/v1/authorize\n      tokenUrl: https://esentire.okta.com/oauth2/v1/token\n      refreshUrl: null\n      scopes:\n        openid: OpenID Connect subject identifier\n        profile:\
  \ End-user profile claims\n        email: End-user email claim\n  pkce:\n    required: true\n    methods:\n    - S256\n  issuer: https://esentire.okta.com\n  identity_provider: Okta\n  applies_to:\n  - https://api.esentire.com/mcp\n  note: >-\n    The only grant type advertised is authorization_code. There is no\n    client_credentials flow in the metadata, which means machine-to-machine access\n    to this surface is not offered through the discovered authorization server —\n    every token is issued against a human Okta identity.\ndynamic_client_registration:\n  supported: true\n  spec: RFC 7591\n  endpoint: https://api.esentire.com/register\n  anonymous: true\n  observed_status: 201\n  token_endpoint_auth_method: none\n  note: >-\n    Registration is open without credentials — an anonymous POST returned 201 with\n    a client_id, `token_endpoint_auth_method: \"none\"` (public client) and scope\n    \"openid profile email\". This is the MCP client-onboarding pattern: an agent can\n \
  \   self-register, but the resulting token still requires a human eSentire login to\n    obtain, so registration alone grants no data access.\ndiscovery:\n  authorization_server_metadata:\n    url: https://api.esentire.com/.well-known/oauth-authorization-server\n    spec: RFC 8414\n    status: 200\n  protected_resource_metadata:\n    url: https://api.esentire.com/.well-known/oauth-protected-resource\n    spec: RFC 9728\n    status: 200\n    resource: https://api.esentire.com\n  challenge:\n    header: 'WWW-Authenticate: Bearer resource_metadata=\"https://api.esentire.com/.well-known/oauth-protected-resource\"'\n    observed_on: https://api.esentire.com/mcp/v1\n    status: 401\nclaims_supported:\n- ver\n- jti\n- iss\n- aud\n- iat\n- exp\n- cid\n- uid\n- scp\n- sub\nopenid_connect:\n  end_session_endpoint: https://esentire.okta.com/oauth2/v1/logout\n  revocation_endpoint: https://esentire.okta.com/oauth2/v1/revoke\n  revocation_endpoint_auth_methods_supported:\n  - none\n  note: >-\n   \
  \ api.esentire.com/.well-known/openid-configuration is NOT served (403). The\n    openid/profile/email scopes and the OIDC endpoints are advertised through the\n    OAuth 2.0 authorization-server metadata document instead.\ngaps:\n- No published authentication documentation. Nothing on esentire.com describes how a customer obtains or rotates a token.\n- No client_credentials or service-account flow is advertised, so unattended integration is not documented as possible.\n- Token lifetime, refresh behaviour, and rate/quota consequences of authentication are undocumented.\nx-evidence:\n  fetched: '2026-08-12'\n  urls:\n  - url: https://api.esentire.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://api.esentire.com/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://api.esentire.com/register\n    status: 201\n  - url: https://api.esentire.com/mcp/v1\n    status: 401\n  - url: https://api.esentire.com/.well-known/openid-configuration\n    status:\
  \ 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esentire/refs/heads/main/authentication/esentire-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Threat Intelligence
- Incident Response
- Model Context Protocol
- Agents
- OAuth
- SaaS
---
