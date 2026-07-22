---
api_key_in: []
api_specs:
- filename: toqio-accounts-openapi.yml
  format: yaml
  label: Toqio Accounts API
  slug: toqio-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-accounts-openapi.yml
- filename: toqio-cards-openapi.yml
  format: yaml
  label: Toqio Cards API
  slug: toqio-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-cards-openapi.yml
- filename: toqio-transactions-openapi.yml
  format: yaml
  label: Toqio Transactions API
  slug: toqio-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-transactions-openapi.yml
- filename: toqio-beneficiaries-openapi.yml
  format: yaml
  label: Toqio Beneficiaries API
  slug: toqio-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-beneficiaries-openapi.yml
- filename: toqio-fees-openapi.yml
  format: yaml
  label: Toqio Fees API
  slug: toqio-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-fees-openapi.yml
- filename: toqio-clients-openapi.yml
  format: yaml
  label: Toqio Clients API
  slug: toqio-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-clients-openapi.yml
- filename: toqio-compliance-endpoints-openapi.yml
  format: yaml
  label: Toqio Compliance API
  slug: toqio-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-compliance-endpoints-openapi.yml
- filename: toqio-upload-kyb-documents-openapi.yml
  format: yaml
  label: Toqio KYB Documents API
  slug: toqio-kyb-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-upload-kyb-documents-openapi.yml
- filename: toqio-create-lead-service-openapi.yml
  format: yaml
  label: Toqio Create Lead API
  slug: toqio-create-lead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-create-lead-service-openapi.yml
- filename: toqio-revenue-collections-openapi.yml
  format: yaml
  label: Toqio Revenue Collections API
  slug: toqio-revenue-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-revenue-collections-openapi.yml
- filename: toqio-custom-notifications-openapi.yml
  format: yaml
  label: Toqio Custom Notifications API
  slug: toqio-custom-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-custom-notifications-openapi.yml
- filename: toqio-security-openapi.yml
  format: yaml
  label: Toqio Security API
  slug: toqio-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-security-openapi.yml
- filename: toqio-integration-hub-api-openapi.yml
  format: yaml
  label: Toqio Integration Hub API
  slug: toqio-integration-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-integration-hub-api-openapi.yml
- filename: toqio-card-management-api-openapi.yml
  format: yaml
  label: Toqio Card Management API (Integration Hub)
  slug: toqio-card-management-api-integration-hub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-card-management-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Toqio Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Toqio secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Toqio
provider_slug: toqio
scheme_count: 3
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: clientCredentials
  sources:
  - openapi/toqio-accounts-openapi.yml
  - openapi/toqio-beneficiaries-openapi.yml
  - openapi/toqio-cards-openapi.yml
  - openapi/toqio-clients-openapi.yml
  - openapi/toqio-compliance-endpoints-openapi.yml
  - openapi/toqio-custom-notifications-openapi.yml
  - openapi/toqio-fees-openapi.yml
  - openapi/toqio-security-openapi.yml
  - openapi/toqio-transactions-openapi.yml
  type: oauth2
- flows:
  - flow: password
    scopes: 0
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: bearer-jwt
  sources:
  - openapi/toqio-cards-openapi.yml
  - openapi/toqio-create-lead-service-openapi.yml
  - openapi/toqio-get-pre-signed-url-openapi.yml
  - openapi/toqio-security-openapi.yml
  - openapi/toqio-upload-kyb-documents-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/toqio-integration-hub-api-openapi.yml
  type: http
slug: toqio-authentication
source_filename: toqio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/toqio-accounts-openapi.yml, openapi/toqio-beneficiaries-openapi.yml, openapi/toqio-cards-openapi.yml,\n  openapi/toqio-clients-openapi.yml, openapi/toqio-compliance-endpoints-openapi.yml, openapi/toqio-create-lead-service-openapi.yml,\n  openapi/toqio-custom-notifications-openapi.yml, openapi/toqio-fees-openapi.yml, openapi/toqio-get-pre-signed-url-openapi.yml,\n  openapi/toqio-integration-hub-api-openapi.yml, openapi/toqio-security-openapi.yml, openapi/toqio-transactions-openapi.yml\n  ...\ndocs:\n  - https://platform.toq.io/reference/authenticating-against-toqio-api\n  - https://integrate.toq.io/reference/authentication\nnotes: >-\n  Platform API: OAuth 2.0 Client Credentials Grant — POST\n  https://api.toq.io/iam/oauth/token with grant_type=client_credentials and\n  HTTP Basic (base64 username:password); access_token is a JWT sent as\n  \"Authorization: Bearer {access_token}\" and expires in 3600 seconds by\n  default\
  \ (customisable on approved request). Integration Hub: layered\n  security model over HTTPS (TLS 1.2 minimum, TLS 1.3 recommended) — Layer 1\n  API Key in the X-Api-Key header (both directions, rotation supported),\n  Layer 2 HMAC-SHA256 payload signature in X-Toqio-Signature\n  (sha256={base64 HMAC over raw body bytes}; absent signature -> 401, invalid\n  -> 403), Layer 3 OAuth 2.0 / OIDC client credentials with self-signed JWT\n  bearer assertions per RFC 7523 (RSA 2048+ or EC P-256/P-384; private key\n  never leaves the integrator).\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - password\nschemes:\n- name: clientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.toq.io/iam/oauth/token\n    scopes: 0\n  sources:\n  - openapi/toqio-accounts-openapi.yml\n  - openapi/toqio-beneficiaries-openapi.yml\n  - openapi/toqio-cards-openapi.yml\n  - openapi/toqio-clients-openapi.yml\n  - openapi/toqio-compliance-endpoints-openapi.yml\n\
  \  - openapi/toqio-custom-notifications-openapi.yml\n  - openapi/toqio-fees-openapi.yml\n  - openapi/toqio-security-openapi.yml\n  - openapi/toqio-transactions-openapi.yml\n- name: bearer-jwt\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://api.toq.io/iam/oauth/token\n    scopes: 0\n  sources:\n  - openapi/toqio-cards-openapi.yml\n  - openapi/toqio-create-lead-service-openapi.yml\n  - openapi/toqio-get-pre-signed-url-openapi.yml\n  - openapi/toqio-security-openapi.yml\n  - openapi/toqio-upload-kyb-documents-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/toqio-integration-hub-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/authentication/toqio-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Embedded Finance
- Fintech
- Banking as a Service
- Payments
- Cards
- Corporate Banking
- Lending
- Compliance
- SMEs
---
