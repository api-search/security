---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Meniga Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Meniga secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Meniga
provider_slug: meniga
scheme_count: 2
schemes:
- flows:
  - authorizationCode
  name: OAuth2
  note: Authorization/token endpoints are tenant-specific (per financial institution).
  sources:
  - https://meniga.github.io/mobile-sdk-ios/
  type: oauth2
- name: OpenIDConnect
  note: OpenID Connect on top of Meniga IdentityServer for claims-based identity.
  sources:
  - https://github.com/meniga/Meniga.IdentityModel
  type: openIdConnect
slug: meniga-authentication
source_filename: meniga-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/meniga/mobile-sdk-ios\ndocs: https://meniga.github.io/mobile-sdk-ios/\nnotes: >-\n  Meniga's REST API is secured with OAuth 2.0 and OpenID Connect. Meniga runs an\n  IdentityServer-based authorization server (see github.com/meniga/Meniga.IdentityServer\n  and Meniga.IdentityModel). The API is tenant/white-label hosted: each bank or\n  financial institution operates its own Meniga API URL and issues authentication\n  credentials to its client applications, which the mobile SDKs pass through to\n  the tenant authorization server. No public OpenAPI securitySchemes were available\n  to derive from (the developer portal at developer.meniga.cloud is access-gated),\n  so this profile was captured from the published SDK documentation rather than a\n  machine-readable spec.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  tenant_hosted: true\nschemes:\n- name: OAuth2\n\
  \  type: oauth2\n  flows:\n  - authorizationCode\n  note: Authorization/token endpoints are tenant-specific (per financial institution).\n  sources:\n  - https://meniga.github.io/mobile-sdk-ios/\n- name: OpenIDConnect\n  type: openIdConnect\n  note: >-\n    OpenID Connect on top of Meniga IdentityServer for claims-based identity.\n  sources:\n  - https://github.com/meniga/Meniga.IdentityModel\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meniga/refs/heads/main/authentication/meniga-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Fintech
- Digital Banking
- Personal Finance Management
- Open Banking
- Transaction Enrichment
- Financial Services
- Banking
- SDK
---
