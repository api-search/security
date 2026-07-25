---
api_key_in: []
api_specs:
- filename: binarly-assistant-api-openapi.yml
  format: yaml
  label: Binarly Assistant API
  slug: binarly-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-assistant-api-openapi.yml
- filename: binarly-chart-api-openapi.yml
  format: yaml
  label: Binarly Chart API
  slug: binarly-chart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-chart-api-openapi.yml
- filename: binarly-customrules-api-openapi.yml
  format: yaml
  label: Binarly CustomRules API
  slug: binarly-customrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-customrules-api-openapi.yml
- filename: binarly-escalation-api-openapi.yml
  format: yaml
  label: Binarly Escalation API
  slug: binarly-escalation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-escalation-api-openapi.yml
- filename: binarly-file-api-openapi.yml
  format: yaml
  label: Binarly File API
  slug: binarly-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-file-api-openapi.yml
- filename: binarly-finding-api-openapi.yml
  format: yaml
  label: Binarly Finding API
  slug: binarly-finding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-finding-api-openapi.yml
- filename: binarly-grid-api-openapi.yml
  format: yaml
  label: Binarly Grid API
  slug: binarly-grid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-grid-api-openapi.yml
- filename: binarly-group-api-openapi.yml
  format: yaml
  label: Binarly Group API
  slug: binarly-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-group-api-openapi.yml
- filename: binarly-image-api-openapi.yml
  format: yaml
  label: Binarly Image API
  slug: binarly-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-image-api-openapi.yml
- filename: binarly-integration-api-openapi.yml
  format: yaml
  label: Binarly Integration API
  slug: binarly-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-integration-api-openapi.yml
- filename: binarly-notification-api-openapi.yml
  format: yaml
  label: Binarly Notification API
  slug: binarly-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-notification-api-openapi.yml
- filename: binarly-product-api-openapi.yml
  format: yaml
  label: Binarly Product API
  slug: binarly-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-product-api-openapi.yml
- filename: binarly-rolebinding-api-openapi.yml
  format: yaml
  label: Binarly RoleBinding API
  slug: binarly-rolebinding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-rolebinding-api-openapi.yml
- filename: binarly-scan-api-openapi.yml
  format: yaml
  label: Binarly Scan API
  slug: binarly-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-scan-api-openapi.yml
- filename: binarly-search-api-openapi.yml
  format: yaml
  label: Binarly Search API
  slug: binarly-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-search-api-openapi.yml
- filename: binarly-subscription-api-openapi.yml
  format: yaml
  label: Binarly Subscription API
  slug: binarly-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-subscription-api-openapi.yml
- filename: binarly-tempfile-api-openapi.yml
  format: yaml
  label: Binarly TempFile API
  slug: binarly-tempfile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-tempfile-api-openapi.yml
- filename: binarly-user-api-openapi.yml
  format: yaml
  label: Binarly User API
  slug: binarly-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-user-api-openapi.yml
- filename: binarly-userstorage-api-openapi.yml
  format: yaml
  label: Binarly UserStorage API
  slug: binarly-userstorage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-userstorage-api-openapi.yml
- filename: binarly-vulnerability-api-openapi.yml
  format: yaml
  label: Binarly Vulnerability API
  slug: binarly-vulnerability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-vulnerability-api-openapi.yml
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
