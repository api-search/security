---
api_key_in:
- header
auth_types:
- http
- oauth2
- openIdConnect
- saml
description: ''
kind: authentication
layout: security
method: searched
name: Regscale Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: RegScale secures its APIs with http, oauth2, openIdConnect, and saml across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: RegScale
provider_slug: regscale
scheme_count: 4
schemes:
- bearerFormat: JWT
  description: Every RegScale API call carries a JSON Web Token in the Authorization header. Interactive tokens are obtained by POSTing credentials to /api/authentication/login on the tenant and are valid for 24 hours, carrying the permissions of the authenticated user. Token validity can be checked at /api/authentication/validateToken.
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - https://regscale.readme.io/reference/regscale-api-documentation
  - 'regscale-cli 6.42.0.0: regscale/core/app/internal/login.py'
  type: http
- bearerFormat: JWT
  description: For unattended and automated integrations, administrators create a Service Account under Admin Panel -> Setup -> Service Accounts, which issues a long-running Personal Access Token (PAT). Service Account tokens inherit Administrator privileges and do not consume a user license. This is the credential the RegScale CLI and the gRPC ingestion services are intended to run under.
  in: header
  name: servicAccountPAT
  parameter: Authorization
  scheme: bearer
  scope: tenant-wide administrator
  sources:
  - https://regscale.readme.io/docs/service-accounts-1
  type: http
- description: RegScale supports Single Sign-On for interactive users over OAuth 2.0 (documented for Microsoft Entra ID / Azure AD and Okta) and SAML, with MFA enforced by the identity provider. SSO governs human sign-in to the tenant; it is not the mechanism used for programmatic API access, which uses the bearer JWT / Service Account PAT above.
  name: sso
  sources:
  - https://regscale.readme.io/docs/setup-single-sign-on-sso
  - https://regscale.readme.io/docs/multi-factor-authentication-mfa
  type: openIdConnect
- description: The rs-data gRPC ingestion clients attach the same Bearer token as call credentials over a TLS channel (grpc.ssl_channel_credentials()); an insecure plaintext channel is available but off by default.
  name: grpcCallCredentials
  scheme: bearer
  sources:
  - 'regscale-cli 6.42.0.0: regscale/core/grpc/client.py'
  transport: grpc-tls
  type: http
slug: regscale-authentication
source_filename: regscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://regscale.readme.io/docs/service-accounts-1\ndocs: https://regscale.readme.io/docs/setup-single-sign-on-sso\nnote: >-\n  Derived from RegScale's published documentation index (regscale.readme.io/llms.txt) and\n  corroborated against the first-party regscale-cli 6.42.0.0 client. There is no publicly\n  retrievable OpenAPI document, so securitySchemes were not read from a spec - every scheme\n  below is grounded in a named documentation page or in RegScale's own client code.\nsummary:\n  types: [http, oauth2, openIdConnect, saml]\n  api_key_in: [header]\n  bearer_format: JWT\n  oauth2_flows: [authorizationCode]\n  oauth2_role: sso-only\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter: Authorization\n  description: >-\n    Every RegScale API call carries a JSON Web Token in the Authorization header. Interactive\n    tokens are obtained by POSTing credentials to\
  \ /api/authentication/login on the tenant and\n    are valid for 24 hours, carrying the permissions of the authenticated user. Token validity\n    can be checked at /api/authentication/validateToken.\n  sources:\n  - https://regscale.readme.io/reference/regscale-api-documentation\n  - 'regscale-cli 6.42.0.0: regscale/core/app/internal/login.py'\n- name: servicAccountPAT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter: Authorization\n  description: >-\n    For unattended and automated integrations, administrators create a Service Account under\n    Admin Panel -> Setup -> Service Accounts, which issues a long-running Personal Access\n    Token (PAT). Service Account tokens inherit Administrator privileges and do not consume\n    a user license. This is the credential the RegScale CLI and the gRPC ingestion services\n    are intended to run under.\n  scope: tenant-wide administrator\n  sources:\n  - https://regscale.readme.io/docs/service-accounts-1\n- name:\
  \ sso\n  type: openIdConnect\n  description: >-\n    RegScale supports Single Sign-On for interactive users over OAuth 2.0 (documented for\n    Microsoft Entra ID / Azure AD and Okta) and SAML, with MFA enforced by the identity\n    provider. SSO governs human sign-in to the tenant; it is not the mechanism used for\n    programmatic API access, which uses the bearer JWT / Service Account PAT above.\n  sources:\n  - https://regscale.readme.io/docs/setup-single-sign-on-sso\n  - https://regscale.readme.io/docs/multi-factor-authentication-mfa\n- name: grpcCallCredentials\n  type: http\n  scheme: bearer\n  transport: grpc-tls\n  description: >-\n    The rs-data gRPC ingestion clients attach the same Bearer token as call credentials over\n    a TLS channel (grpc.ssl_channel_credentials()); an insecure plaintext channel is\n    available but off by default.\n  sources:\n  - 'regscale-cli 6.42.0.0: regscale/core/grpc/client.py'\nunauthorized_behaviour:\n  '401': unauthenticated - token missing,\
  \ expired or invalid\n  '403': unauthorized - authenticated but lacking the required role or permission\n  source: https://regscale.readme.io/reference/regscale-api-documentation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regscale/refs/heads/main/authentication/regscale-authentication.yml
summary_line: http/oauth2/openIdConnect/saml · 4 schemes
tags:
- Company
- Compliance
- Governance Risk and Compliance
- Continuous Controls Monitoring
- Security
- FedRAMP
- OSCAL
- Risk Management
- Audit
- Compliance as Code
- Vulnerability Management
- Government
---
