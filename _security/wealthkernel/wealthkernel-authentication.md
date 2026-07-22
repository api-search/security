---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: WealthKernel secures its API with OAuth2 client-credentials against an OpenID Connect authorization server (Duende/IdentityServer-style "/connect/token" endpoint). API clients and secrets are created and managed by Dashboard admin users under Configuration -> API clients. The client_id (client key) and client_secret are exchanged at the token endpoint for a short-lived access token, which is then sent as a Bearer token on each API request. Sandbox and production use separate authorization servers.
kind: authentication
layout: security
method: searched
name: Wealthkernel Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: WealthKernel secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: WealthKernel
provider_slug: wealthkernel
scheme_count: 1
schemes:
- environments:
  - api_base: https://api.wealthkernel.io
    env: production
    issuer: https://auth.wealthkernel.com/
    jwks_uri: https://auth.wealthkernel.com/.well-known/openid-configuration/jwks
    token_url: https://auth.wealthkernel.com/connect/token
  - api_base: https://api.sandbox.wealthkernel.io
    env: sandbox
    issuer: https://auth.sandbox.wealthkernel.io/
    jwks_uri: https://auth.sandbox.wealthkernel.io/.well-known/openid-configuration/jwks
    token_url: https://auth.sandbox.wealthkernel.io/connect/token
  flow: clientCredentials
  grant_types_supported:
  - client_credentials
  name: OAuth2ClientCredentials
  scopes_supported:
  - openid
  sources:
  - well-known/wealthkernel-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - private_key_jwt
  - client_secret_basic
  type: oauth2
slug: wealthkernel-authentication
source_filename: wealthkernel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://auth.wealthkernel.com/.well-known/openid-configuration\ndocs: https://docs.wealthkernel.com/docs/api/getting-started\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\n  token_endpoint_auth: [client_secret_post, private_key_jwt, client_secret_basic]\ndescription: >-\n  WealthKernel secures its API with OAuth2 client-credentials against an OpenID Connect authorization\n  server (Duende/IdentityServer-style \"/connect/token\" endpoint). API clients and secrets are created\n  and managed by Dashboard admin users under Configuration -> API clients. The client_id (client key)\n  and client_secret are exchanged at the token endpoint for a short-lived access token, which is then\n  sent as a Bearer token on each API request. Sandbox and production use separate authorization servers.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  environments:\n\
  \  - env: production\n    issuer: https://auth.wealthkernel.com/\n    token_url: https://auth.wealthkernel.com/connect/token\n    jwks_uri: https://auth.wealthkernel.com/.well-known/openid-configuration/jwks\n    api_base: https://api.wealthkernel.io\n  - env: sandbox\n    issuer: https://auth.sandbox.wealthkernel.io/\n    token_url: https://auth.sandbox.wealthkernel.io/connect/token\n    jwks_uri: https://auth.sandbox.wealthkernel.io/.well-known/openid-configuration/jwks\n    api_base: https://api.sandbox.wealthkernel.io\n  grant_types_supported: [client_credentials]\n  scopes_supported: [openid]\n  token_endpoint_auth_methods_supported: [client_secret_post, private_key_jwt, client_secret_basic]\n  sources: [well-known/wealthkernel-openid-configuration.json]\naccess_token:\n  transport: Authorization Bearer header\n  type: JWT (signed by the authorization server; verifiable via jwks_uri)\ncredential_management:\n  where: WealthKernel Dashboard -> Configuration -> API clients\n  docs:\
  \ https://docs.wealthkernel.com/docs/guides/docs/api-clients/Managing-Secrets.md\n  notes: Admin users generate and rotate client secrets; secrets are shown once and must be stored securely.\nip_allow_listing:\n  supported: true\n  docs: https://docs.wealthkernel.com/docs/guides/docs/ip-allow-listing/Basics.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealthkernel/refs/heads/main/authentication/wealthkernel-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Investing
- Wealth Management
- Brokerage
- Custody
- Fintech
- Investment API
- Embedded Finance
- ISA
- SIPP
- Banking as a Service
- United Kingdom
- Europe
---
