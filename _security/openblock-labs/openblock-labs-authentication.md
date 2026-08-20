---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Openblock Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenBlock Labs declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: OpenBlock Labs
provider_slug: openblock-labs
scheme_count: 0
schemes: []
slug: openblock-labs-authentication
source_filename: openblock-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://auth.openblocklabs.com/.well-known/openid-configuration\ndocs: https://auth.openblocklabs.com/.well-known/oauth-authorization-server\nprovider: OpenBlock Labs (OB-1)\nsummary: >-\n  OB-1 authenticates via a standards-compliant OAuth 2.0 / OpenID Connect\n  authorization server hosted at auth.openblocklabs.com (WorkOS AuthKit).\n  Interactive users sign in through AuthKit; programmatic/machine access is\n  available via the client_credentials and OAuth 2.0 Device Authorization\n  grants. Enterprise deployments additionally support SSO / SAML.\nsecurity_schemes:\n- type: oauth2\n  name: OB-1 OAuth 2.0 / OIDC\n  issuer: https://auth.openblocklabs.com\n  flows:\n  - grant: authorization_code\n    pkce: true\n    pkce_methods: [S256]\n    authorization_endpoint: https://auth.openblocklabs.com/oauth2/authorize\n    token_endpoint: https://auth.openblocklabs.com/oauth2/token\n  - grant: client_credentials\n    token_endpoint:\
  \ https://auth.openblocklabs.com/oauth2/token\n  - grant: refresh_token\n    token_endpoint: https://auth.openblocklabs.com/oauth2/token\n  - grant: urn:ietf:params:oauth:grant-type:device_code\n    device_authorization_endpoint: https://auth.openblocklabs.com/oauth2/device_authorization\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  dynamic_client_registration: https://auth.openblocklabs.com/oauth2/register\n  introspection_endpoint: https://auth.openblocklabs.com/oauth2/introspection\n  userinfo_endpoint: https://auth.openblocklabs.com/oauth2/userinfo\n  jwks_uri: https://auth.openblocklabs.com/oauth2/jwks\n  id_token_signing_alg: [RS256]\n  scopes: [openid, profile, email, offline_access]\n- type: openIdConnect\n  name: OB-1 OpenID Connect\n  openIdConnectUrl: https://auth.openblocklabs.com/.well-known/openid-configuration\nenterprise:\n  sso_saml: true\n  note: Enterprise plans support SSO / SAML with major identity providers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openblock-labs/refs/heads/main/authentication/openblock-labs-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Data
- Coding Agents
- AI Agents
- Developer Tools
- Automation
- Authentication
- MCP
---
