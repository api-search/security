---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: assinafy-com-br-accounts-api-openapi.yml
  format: yaml
  label: Assinafy Accounts API
  slug: assinafy-com-br-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-accounts-api-openapi.yml
- filename: assinafy-com-br-assignments-api-openapi.yml
  format: yaml
  label: Assinafy Assignments API
  slug: assinafy-com-br-assignments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-assignments-api-openapi.yml
- filename: assinafy-com-br-authentication-api-openapi.yml
  format: yaml
  label: Assinafy Authentication API
  slug: assinafy-com-br-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-authentication-api-openapi.yml
- filename: assinafy-com-br-contracts-api-openapi.yml
  format: yaml
  label: Assinafy Contracts API
  slug: assinafy-com-br-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-contracts-api-openapi.yml
- filename: assinafy-com-br-documents-api-openapi.yml
  format: yaml
  label: Assinafy Documents API
  slug: assinafy-com-br-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-documents-api-openapi.yml
- filename: assinafy-com-br-fields-api-openapi.yml
  format: yaml
  label: Assinafy Fields API
  slug: assinafy-com-br-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-fields-api-openapi.yml
- filename: assinafy-com-br-oauth-api-openapi.yml
  format: yaml
  label: Assinafy OAuth API
  slug: assinafy-com-br-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-oauth-api-openapi.yml
- filename: assinafy-com-br-signers-api-openapi.yml
  format: yaml
  label: Assinafy Signers API
  slug: assinafy-com-br-signers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-signers-api-openapi.yml
- filename: assinafy-com-br-signing-api-openapi.yml
  format: yaml
  label: Assinafy Signing API
  slug: assinafy-com-br-signing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-signing-api-openapi.yml
- filename: assinafy-com-br-tags-api-openapi.yml
  format: yaml
  label: Assinafy Tags API
  slug: assinafy-com-br-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-tags-api-openapi.yml
- filename: assinafy-com-br-templates-api-openapi.yml
  format: yaml
  label: Assinafy Templates API
  slug: assinafy-com-br-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-templates-api-openapi.yml
- filename: assinafy-com-br-users-api-openapi.yml
  format: yaml
  label: Assinafy Users API
  slug: assinafy-com-br-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-users-api-openapi.yml
- filename: assinafy-com-br-webhook-payloads-api-openapi.yml
  format: yaml
  label: Assinafy Webhook Payloads API
  slug: assinafy-com-br-webhook-payloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-webhook-payloads-api-openapi.yml
- filename: assinafy-com-br-webhooks-api-openapi.yml
  format: yaml
  label: Assinafy Webhooks API
  slug: assinafy-com-br-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Assinafy Com Br Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Assinafy secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Assinafy
provider_slug: assinafy-com-br
scheme_count: 4
schemes:
- bearerFormat: JWT
  description: 'Access token: `Authorization: Bearer {access_token}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/assinafy-com-br-openapi.json
  type: http
- description: Permanent API key (recommended for back-end integrations).
  in: header
  name: apiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/assinafy-com-br-openapi.json
  type: apiKey
- description: 'Signer access code used by signer-facing (Signing) endpoints instead of a user token: the code in the signer''s signing link, sent as the `signer-access-code` query or body parameter. It can be used again and has no expiry; it stops working when the signing request is removed. Treat it as a secret.'
  in: query
  name: signerAccessCode
  parameter: signer-access-code
  sources:
  - openapi/assinafy-com-br-openapi.json
  type: apiKey
- description: OAuth 2.1 authorization code flow with mandatory PKCE (S256), for applications and AI assistants acting in a user's workspace with that user's permission — as opposed to `apiKeyAuth`/`bearerAuth`, which authenticate the workspace or user directly. A token carries only the scopes the user approved and works for one workspace. Endpoints are published by the authorization server at `https://auth.assi
  flows:
  - authorizationUrl: https://auth.assinafy.com.br/oauth/authorize
    flow: authorizationCode
    scopes: 10
    tokenUrl: https://api.assinafy.com.br/v1/oauth/token
  name: oauth2
  sources:
  - openapi/assinafy-com-br-openapi.json
  type: oauth2
slug: assinafy-com-br-authentication
source_filename: assinafy-com-br-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/assinafy-com-br-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Access token: `Authorization: Bearer {access_token}`.'\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Permanent API key (recommended for back-end integrations).\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n- name: signerAccessCode\n  type: apiKey\n  in: query\n  parameter: signer-access-code\n  description: 'Signer access code used by signer-facing (Signing) endpoints instead of a user\n    token: the code in the signer''s signing link, sent as the `signer-access-code` query or\n    body parameter. It can be used again and has no expiry; it stops working when\
  \ the signing\n    request is removed. Treat it as a secret.'\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.assinafy.com.br/oauth/authorize\n    tokenUrl: https://api.assinafy.com.br/v1/oauth/token\n    scopes: 10\n  description: OAuth 2.1 authorization code flow with mandatory PKCE (S256), for applications\n    and AI assistants acting in a user's workspace with that user's permission — as opposed\n    to `apiKeyAuth`/`bearerAuth`, which authenticate the workspace or user directly. A token\n    carries only the scopes the user approved and works for one workspace. Endpoints are published\n    by the authorization server at `https://auth.assi\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/assinafy-com-br/authentication/assinafy-com-br-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- E-Signature
- Document Management
- Brazil
- Free
---
