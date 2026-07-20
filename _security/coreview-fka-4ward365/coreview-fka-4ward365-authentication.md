---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Coreview Fka 4Ward365 Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CoreView (FKA 4ward365) secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CoreView (FKA 4ward365)
provider_slug: coreview-fka-4ward365
scheme_count: 2
schemes:
- client_auth: Basic (base64 client_id:client_secret) with grant_type=client_credentials
  credentials: Client ID and Client Secret issued by CoreView Support
  flow: clientCredentials
  gov_token_url: https://usidentity.coreview.com/connect/token
  name: OAuth2ClientCredentials
  sources:
  - https://help.coreview.com/api-authentication
  token_url: https://identity.coreview.com/connect/token
  type: oauth2
- endpoints:
    authorization: https://identity.coreview.com/connect/authorize
    introspection: https://identity.coreview.com/connect/introspect
    jwks: https://identity.coreview.com/.well-known/openid-configuration/jwks
    revocation: https://identity.coreview.com/connect/revocation
    token: https://identity.coreview.com/connect/token
    userinfo: https://identity.coreview.com/connect/userinfo
  grant_types_supported:
  - client_credentials
  - authorization_code
  - refresh_token
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  issuer: https://identity.coreview.com
  name: OpenIDConnect
  openIdConnectUrl: https://identity.coreview.com/.well-known/openid-configuration
  sources:
  - https://identity.coreview.com/.well-known/openid-configuration
  type: openIdConnect
slug: coreview-fka-4ward365-authentication
source_filename: coreview-fka-4ward365-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://help.coreview.com/api-authentication\ndocs: https://help.coreview.com/api-authentication\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  token_type: Bearer JWT\n  token_ttl_seconds: 3600\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://identity.coreview.com/connect/token\n  gov_token_url: https://usidentity.coreview.com/connect/token\n  client_auth: Basic (base64 client_id:client_secret) with grant_type=client_credentials\n  credentials: Client ID and Client Secret issued by CoreView Support\n  sources:\n  - https://help.coreview.com/api-authentication\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://identity.coreview.com/.well-known/openid-configuration\n  issuer: https://identity.coreview.com\n  grant_types_supported:\n  - client_credentials\n  - authorization_code\n\
  \  - refresh_token\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  endpoints:\n    authorization: https://identity.coreview.com/connect/authorize\n    token: https://identity.coreview.com/connect/token\n    userinfo: https://identity.coreview.com/connect/userinfo\n    introspection: https://identity.coreview.com/connect/introspect\n    revocation: https://identity.coreview.com/connect/revocation\n    jwks: https://identity.coreview.com/.well-known/openid-configuration/jwks\n  sources:\n  - https://identity.coreview.com/.well-known/openid-configuration\nnotes: >-\n  CoreView Public APIs are secured with OAuth 2.0 / OpenID Connect using the\n  client-credentials grant against the CoreView IdentityServer. Requests to the\n  regional API proxy carry an Authorization: Bearer <JWT> header and an\n  X-scompany-ID header identifying the CoreView company/tenant. Tokens expire\n  after 3600 seconds and must be refreshed. GOV (FedRAMP) tenants\
  \ use the\n  usidentity.coreview.com identity host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coreview-fka-4ward365/refs/heads/main/authentication/coreview-fka-4ward365-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Microsoft 365
- SaaS Management
- Governance
- Security
- Identity
- Automation
- Workflow
- License Management
- IT Operations
---
