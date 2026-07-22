---
api_key_in:
- header
auth_types:
- oauth2
- openIdConnect
- apiKey
- saml
description: ''
kind: authentication
layout: security
method: searched
name: Matchory Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- tokenExchange
overview: Matchory secures its APIs with oauth2, openIdConnect, apiKey, and saml across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, and tokenExchange flow(s).
provider_name: Matchory
provider_slug: matchory
scheme_count: 4
schemes:
- flows:
  - authorizationUrl: https://discovery.matchory.com/auth/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://discovery.matchory.com/auth/oauth/token
  - flow: clientCredentials
    tokenUrl: https://discovery.matchory.com/auth/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:token-exchange
  id_token_signing_alg:
  - RS256
  issuer: https://matchory.com
  jwks_uri: https://discovery.matchory.com/.well-known/jwks.json
  name: OAuth2
  registration_endpoint: https://discovery.matchory.com/auth/oauth/register
  revocation_endpoint: https://discovery.matchory.com/auth/oauth/revoke
  source: well-known/matchory-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - none
  type: oauth2
  userinfo_endpoint: https://discovery.matchory.com/auth/userinfo
- name: OpenIDConnect
  openIdConnectUrl: https://discovery.matchory.com/.well-known/openid-configuration
  scopes:
  - openid
  - profile
  - email
  - mcp:use
  source: well-known/matchory-openid-configuration.json
  type: openIdConnect
- description: Role-scoped API keys for programmatic REST/GraphQL access, with role-based access control and full audit trails (documented on the technology page).
  in: header
  name: APIKey
  source: https://matchory.com/en/technology
  type: apiKey
- description: Enterprise single sign-on via SAML 2.0 and OIDC, with just-in-time provisioning and role mapping.
  name: SSO
  source: https://matchory.com/en/technology
  type: saml
slug: matchory-authentication
source_filename: matchory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://discovery.matchory.com/.well-known/openid-configuration\ndocs: https://matchory.com/en/technology\nsummary:\n  types: [oauth2, openIdConnect, apiKey, saml]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken, tokenExchange]\n  pkce: [S256]\n  sso: [SAML 2.0, OIDC]\nschemes:\n- name: OAuth2\n  type: oauth2\n  issuer: https://matchory.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://discovery.matchory.com/auth/oauth/authorize\n    tokenUrl: https://discovery.matchory.com/auth/oauth/token\n    code_challenge_methods: [S256]\n  - flow: clientCredentials\n    tokenUrl: https://discovery.matchory.com/auth/oauth/token\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic, none]\n  grant_types: [authorization_code, refresh_token, client_credentials, 'urn:ietf:params:oauth:grant-type:token-exchange']\n  registration_endpoint: https://discovery.matchory.com/auth/oauth/register\n\
  \  revocation_endpoint: https://discovery.matchory.com/auth/oauth/revoke\n  userinfo_endpoint: https://discovery.matchory.com/auth/userinfo\n  jwks_uri: https://discovery.matchory.com/.well-known/jwks.json\n  id_token_signing_alg: [RS256]\n  source: well-known/matchory-openid-configuration.json\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://discovery.matchory.com/.well-known/openid-configuration\n  scopes: [openid, profile, email, mcp:use]\n  source: well-known/matchory-openid-configuration.json\n- name: APIKey\n  type: apiKey\n  in: header\n  description: >-\n    Role-scoped API keys for programmatic REST/GraphQL access, with role-based\n    access control and full audit trails (documented on the technology page).\n  source: https://matchory.com/en/technology\n- name: SSO\n  type: saml\n  description: >-\n    Enterprise single sign-on via SAML 2.0 and OIDC, with just-in-time\n    provisioning and role mapping.\n  source: https://matchory.com/en/technology\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matchory/refs/heads/main/authentication/matchory-authentication.yml
summary_line: oauth2/openIdConnect/apiKey/saml · 4 schemes
tags:
- Company
- Procurement
- Supplier Discovery
- Sourcing
- Supply Chain
- Data Enrichment
- Entity Resolution
- Market Intelligence
- Risk Management
- MCP
---
