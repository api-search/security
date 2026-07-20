---
api_key_in: []
api_specs:
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Payment Intent API
  slug: ziina-payment-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Refund API
  slug: ziina-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Transfer API
  slug: ziina-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Webhooks API
  slug: ziina-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Account API
  slug: ziina-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ziina Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ziina secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ziina
provider_slug: ziina
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearer
  notes: 'All Ziina API calls authenticate with an HTTP bearer token in the Authorization header (Authorization: Bearer <token>). The token is a JWT access token issued by Ziina''s OAuth 2.0 authorization server.'
  scheme: bearer
  sources:
  - openapi/ziina-openapi.yml
  type: http
- authorizationUrl: https://auth.ziina.com/oidc/auth
  flow: authorization_code
  grantTypes:
  - authorization_code
  - refresh_token
  name: oauth2
  notes: Ziina uses an OIDC-based OAuth 2.0 flow (auth.ziina.com/oidc). Business integration credentials (client_id, username, password) and allowed redirect URIs are provisioned by contacting Ziina support. A personal access token obtained on the Ziina business connect page carries all available scopes for self-integration.
  scopes:
    offline_access: Receive a refresh_token for long-lived access.
    read_account: Read the connected account profile (GET /account).
    write_payment_intents: Create payment intents and accept payments on the account's behalf.
    write_refunds: Issue refunds against payment intents.
    write_transfers: Initiate transfers between Ziina accounts.
    write_webhooks: Register and delete webhook endpoints.
  sources:
  - https://docs.ziina.com/developers/oauth-2.0
  - https://docs.ziina.com/business/oauth-2.0
  tokenUrl: https://auth.ziina.com/oidc/token
  type: oauth2
slug: ziina-authentication
source_filename: ziina-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/ziina-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ziina-openapi.yml\n  notes: >-\n    All Ziina API calls authenticate with an HTTP bearer token in the\n    Authorization header (Authorization: Bearer <token>). The token is a JWT\n    access token issued by Ziina's OAuth 2.0 authorization server.\n- name: oauth2\n  type: oauth2\n  flow: authorization_code\n  authorizationUrl: https://auth.ziina.com/oidc/auth\n  tokenUrl: https://auth.ziina.com/oidc/token\n  grantTypes:\n  - authorization_code\n  - refresh_token\n  scopes:\n    read_account: Read the connected account profile (GET /account).\n    write_payment_intents: Create payment intents and accept payments on the account's behalf.\n    write_refunds: Issue refunds against payment intents.\n    write_transfers: Initiate transfers between Ziina accounts.\n\
  \    write_webhooks: Register and delete webhook endpoints.\n    offline_access: Receive a refresh_token for long-lived access.\n  sources:\n  - https://docs.ziina.com/developers/oauth-2.0\n  - https://docs.ziina.com/business/oauth-2.0\n  notes: >-\n    Ziina uses an OIDC-based OAuth 2.0 flow (auth.ziina.com/oidc). Business\n    integration credentials (client_id, username, password) and allowed redirect\n    URIs are provisioned by contacting Ziina support. A personal access token\n    obtained on the Ziina business connect page carries all available scopes for\n    self-integration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/authentication/ziina-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Payments
- Fintech
- UAE
- MENA
- Money Transfer
- Wallet
---
