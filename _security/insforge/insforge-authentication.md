---
api_key_in:
- header
api_specs:
- filename: insforge-auth-openapi.yaml
  format: yaml
  label: Insforge Authentication API
  slug: insforge-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-auth-openapi.yaml
- filename: insforge-payments-openapi.yaml
  format: yaml
  label: Insforge Payments API
  slug: insforge-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-payments-openapi.yaml
- filename: insforge-storage-openapi.yaml
  format: yaml
  label: Insforge Storage API
  slug: insforge-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-storage-openapi.yaml
- filename: insforge-deployments-openapi.yaml
  format: yaml
  label: Insforge Deployments API
  slug: insforge-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-deployments-openapi.yaml
- filename: insforge-realtime-openapi.yaml
  format: yaml
  label: Insforge Realtime API
  slug: insforge-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-realtime-openapi.yaml
- filename: insforge-functions-openapi.yaml
  format: yaml
  label: Insforge Functions API
  slug: insforge-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-functions-openapi.yaml
- filename: insforge-ai-openapi.yaml
  format: yaml
  label: Insforge AI API
  slug: insforge-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-ai-openapi.yaml
- filename: insforge-tables-openapi.yaml
  format: yaml
  label: Insforge Tables API
  slug: insforge-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-tables-openapi.yaml
- filename: insforge-records-openapi.yaml
  format: yaml
  label: Insforge Records API
  slug: insforge-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-records-openapi.yaml
- filename: insforge-metadata-openapi.yaml
  format: yaml
  label: Insforge Metadata API
  slug: insforge-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-metadata-openapi.yaml
- filename: insforge-secrets-openapi.yaml
  format: yaml
  label: Insforge Secrets API
  slug: insforge-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-secrets-openapi.yaml
- filename: insforge-email-openapi.yaml
  format: yaml
  label: Insforge Email API
  slug: insforge-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-email-openapi.yaml
- filename: insforge-logs-openapi.yaml
  format: yaml
  label: Insforge Logs API
  slug: insforge-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-logs-openapi.yaml
- filename: insforge-health-openapi.yaml
  format: yaml
  label: Insforge Health API
  slug: insforge-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-health-openapi.yaml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Insforge Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
overview: Insforge secures its APIs with apiKey, http, and oauth2 across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and deviceCode flow(s).
provider_name: Insforge
provider_slug: insforge
scheme_count: 7
schemes:
- flows:
    authorizationCode:
      authorizationUrl: https://api.insforge.dev/api/oauth/v1/authorize
      pkce:
      - S256
      - plain
      tokenUrl: https://api.insforge.dev/api/oauth/v1/token
    deviceCode:
      deviceAuthorizationUrl: https://api.insforge.dev/api/oauth/v1/device_authorization
      tokenUrl: https://api.insforge.dev/api/oauth/v1/token
  name: OAuth2
  note: OAuth 2.0 is advertised via RFC 8414 authorization-server metadata, not in the per-service OpenAPI specs.
  scope_count: 11
  scopes_artifact: scopes/insforge-scopes.yml
  source: https://api.insforge.dev/.well-known/oauth-authorization-server
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/insforge-ai-openapi.yaml
  - openapi/insforge-auth-openapi.yaml
  - openapi/insforge-deployments-openapi.yaml
  - openapi/insforge-email-openapi.yaml
  - openapi/insforge-functions-openapi.yaml
  - openapi/insforge-logs-openapi.yaml
  - openapi/insforge-metadata-openapi.yaml
  - openapi/insforge-payments-openapi.yaml
  - openapi/insforge-realtime-openapi.yaml
  - openapi/insforge-records-openapi.yaml
  - openapi/insforge-secrets-openapi.yaml
  - openapi/insforge-tables-openapi.yaml
  type: http
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/insforge-auth-openapi.yaml
  - openapi/insforge-deployments-openapi.yaml
  - openapi/insforge-payments-openapi.yaml
  - openapi/insforge-records-openapi.yaml
  - openapi/insforge-storage-openapi.yaml
  type: apiKey
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/insforge-metadata-openapi.yaml
  - openapi/insforge-realtime-openapi.yaml
  - openapi/insforge-tables-openapi.yaml
  type: apiKey
- in: header
  name: stripeSignature
  parameter: stripe-signature
  sources:
  - openapi/insforge-payments-openapi.yaml
  type: apiKey
- in: header
  name: razorpaySignature
  parameter: x-razorpay-signature
  sources:
  - openapi/insforge-payments-openapi.yaml
  type: apiKey
- description: 'AWS SigV4 authentication using S3 access keys minted by

    `POST /api/storage/s3/access-keys`. Region must match the server''s

    `AWS_REGION` (default `us-east-2`); service scope must be `s3`.'
  name: s3SigV4
  scheme: aws4-hmac-sha256
  sources:
  - openapi/insforge-storage-openapi.yaml
  type: http
slug: insforge-authentication
source_filename: insforge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/*.yaml + https://api.insforge.dev/.well-known/oauth-authorization-server\ndocs: https://docs.insforge.dev/core-concepts/authentication/overview\nagent_auth:\n  supported: true\n  method: identity_assertion (WorkOS ID-JAG)\n  register_uri: https://api.insforge.dev/agent/auth\n  credential_type: api_key (uak_ user API key)\n  skill: https://api.insforge.dev/auth.md\n  note: >-\n    Autonomous agent registration (preview) — a participating provider mints a\n    WorkOS ID-JAG carrying the user's verified email; InsForge exchanges it for a\n    uak_ user API key with no human sign-up form.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - deviceCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://api.insforge.dev/.well-known/oauth-authorization-server\n  flows:\n    authorizationCode:\n      authorizationUrl: https://api.insforge.dev/api/oauth/v1/authorize\n\
  \      tokenUrl: https://api.insforge.dev/api/oauth/v1/token\n      pkce: [S256, plain]\n    deviceCode:\n      deviceAuthorizationUrl: https://api.insforge.dev/api/oauth/v1/device_authorization\n      tokenUrl: https://api.insforge.dev/api/oauth/v1/token\n  scope_count: 11\n  scopes_artifact: scopes/insforge-scopes.yml\n  note: OAuth 2.0 is advertised via RFC 8414 authorization-server metadata, not in the per-service OpenAPI specs.\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/insforge-ai-openapi.yaml\n  - openapi/insforge-auth-openapi.yaml\n  - openapi/insforge-deployments-openapi.yaml\n  - openapi/insforge-email-openapi.yaml\n  - openapi/insforge-functions-openapi.yaml\n  - openapi/insforge-logs-openapi.yaml\n  - openapi/insforge-metadata-openapi.yaml\n  - openapi/insforge-payments-openapi.yaml\n  - openapi/insforge-realtime-openapi.yaml\n  - openapi/insforge-records-openapi.yaml\n  - openapi/insforge-secrets-openapi.yaml\n  - openapi/insforge-tables-openapi.yaml\n\
  - name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/insforge-auth-openapi.yaml\n  - openapi/insforge-deployments-openapi.yaml\n  - openapi/insforge-payments-openapi.yaml\n  - openapi/insforge-records-openapi.yaml\n  - openapi/insforge-storage-openapi.yaml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/insforge-metadata-openapi.yaml\n  - openapi/insforge-realtime-openapi.yaml\n  - openapi/insforge-tables-openapi.yaml\n- name: stripeSignature\n  type: apiKey\n  in: header\n  parameter: stripe-signature\n  sources:\n  - openapi/insforge-payments-openapi.yaml\n- name: razorpaySignature\n  type: apiKey\n  in: header\n  parameter: x-razorpay-signature\n  sources:\n  - openapi/insforge-payments-openapi.yaml\n- name: s3SigV4\n  type: http\n  scheme: aws4-hmac-sha256\n  description: |-\n    AWS SigV4 authentication using S3 access keys minted by\n    `POST /api/storage/s3/access-keys`. Region must match the\
  \ server's\n    `AWS_REGION` (default `us-east-2`); service scope must be `s3`.\n  sources:\n  - openapi/insforge-storage-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/authentication/insforge-authentication.yml
summary_line: apiKey/http/oauth2 · 7 schemes
tags:
- Company
- Backend as a Service
- Agent Native
- Cloud Infrastructure
- Database
- Authentication
- Storage
- Serverless
- Edge Functions
- AI Gateway
- Payments
- Realtime
- Open Source
- Y Combinator
---
