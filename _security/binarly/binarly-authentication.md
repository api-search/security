---
api_key_in: []
api_specs:
- filename: binarly-openapi-original.yml
  format: yaml
  label: Binarly Transparency Platform API
  slug: binarly-transparency-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-openapi-original.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Binarly Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Binarly secures its APIs with http and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Binarly
provider_slug: binarly
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'All API requests present a Keycloak-issued JWT access token in the Authorization: Bearer <token> header. Tokens expire after 30 minutes (expires_in 1800); automation should refresh before each job or on 401.'
  name: auth
  scheme: bearer
  sources:
  - openapi/binarly-openapi-original.yml
  type: http
slug: binarly-authentication
source_filename: binarly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/binarly-openapi-original.yml\ndocs: https://docs.binarly.io/api-reference/authentication/generate-token\nsummary:\n  types:\n  - http\n  - openIdConnect\n  bearer_format: JWT\n  identity_provider: Keycloak (realm BinarlyRealm)\n  oauth2_flows:\n  - clientCredentials\n  - password\nschemes:\n- name: auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    All API requests present a Keycloak-issued JWT access token in the\n    Authorization: Bearer <token> header. Tokens expire after 30 minutes\n    (expires_in 1800); automation should refresh before each job or on 401.\n  sources:\n  - openapi/binarly-openapi-original.yml\noidc:\n  provider: Keycloak\n  realm: BinarlyRealm\n  token_endpoint: https://auth-{slug}.binarly.cloud/realms/BinarlyRealm/protocol/openid-connect/token\n  admin_console: https://<keycloak-host>/admin\n  notes: SaaS auth host is auth-{slug}.binarly.cloud; on-prem customers\
  \ run their own Keycloak.\nflows:\n- flow: clientCredentials\n  audience: machine-to-machine (CI/CD, automation)\n  grant_type: client_credentials\n  client_id: per-tenant service-account client (e.g. BinarlyClient)\n  scope: openid\n  provisioning: >-\n    SaaS customers request client_id/client_secret from support@binarly.io;\n    on-prem customers create the client directly in Keycloak (service accounts roles).\n- flow: password\n  audience: interactive user / ad-hoc scripts\n  grant_type: password\n  client_id: BinarlyClient\n  scope: openid\n  notes: >-\n    Ties API usage to an individual BTP user and respects RBAC. Does NOT work with\n    SSO (SAML / OIDC federation) — requires a dedicated Keycloak username/password.\nrbac:\n  model: role-based access control with per-operation permissions\n  source: x-permission on OpenAPI operations (e.g. products.view, products.create)\n  docs: https://docs.binarly.io/user-guides/rbac/roles\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/authentication/binarly-authentication.yml
summary_line: http/openIdConnect · 1 scheme
tags:
- Company
- Security
- Firmware Security
- Supply Chain Security
- Vulnerability Management
- SBOM
- Binary Analysis
- Post-Quantum Cryptography
- UEFI
- DevSecOps
---
