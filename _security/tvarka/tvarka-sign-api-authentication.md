---
api_key_in:
- header
api_specs:
- filename: tvarka-atk-api-auth-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Auth API
  slug: tvarka-atk-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-auth-api-openapi.yml
- filename: tvarka-atk-api-erasure-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Erasure API
  slug: tvarka-atk-api-erasure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-erasure-api-openapi.yml
- filename: tvarka-atk-api-ltv-api-openapi.yml
  format: yaml
  label: Tvarka ATK API LTV API
  slug: tvarka-atk-api-ltv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-ltv-api-openapi.yml
- filename: tvarka-atk-api-pairing-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Pairing API
  slug: tvarka-atk-api-pairing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-pairing-api-openapi.yml
- filename: tvarka-atk-api-sign-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Sign API
  slug: tvarka-atk-api-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-sign-api-openapi.yml
- filename: auth.json
  format: json
  label: Tvarka ATK API Tvarka ATK API API
  slug: tvarka-atk-api-tvarka-atk-api-api
  spec_type: Postman
  url: https://atk.tvarka.pro/postman/auth.json
- filename: auth.json
  format: json
  label: Tvarka ATK API Tvarka ATK QES Signing API (paid Tier Addendum) API
  slug: tvarka-atk-api-tvarka-atk-qes-signing-api-paid-tier-addendum-api
  spec_type: Postman
  url: https://atk.tvarka.pro/postman/auth.json
- filename: tvarka-atk-api-validation-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Validation API
  slug: tvarka-atk-api-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-validation-api-openapi.yml
- filename: tvarka-atk-api-well-known-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Well Known API
  slug: tvarka-atk-api-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-well-known-api-openapi.yml
- filename: tvarka-sign-api-openapi.yml
  format: yaml
  label: Tvarka Sign API
  slug: tvarka-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-sign-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tvarka Sign Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tvarka ATK API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tvarka ATK API
provider_slug: tvarka
scheme_count: 1
schemes:
- description: Keys are provisioned by Tvarka during onboarding and shown once. A tsk_live_ key acts on production; a tsk_test_ key is the sandbox.
  header: 'Authorization: Bearer <key>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tvarka-sign-api-openapi.yml
  type: http
slug: tvarka-sign-api-authentication
source_filename: tvarka-sign-api-authentication.yml
source_heading: Authentication Profile
source_url: https://sign-api.tvarka.pro/docs
source_yaml: "generated: '2026-08-31'\nmethod: searched\nsource: https://sign-api.tvarka.pro/docs\nsources:\n  - https://sign-api.tvarka.pro/docs\n  - https://sign-api.tvarka.pro/llms.txt\n  - openapi/tvarka-sign-api-openapi.yml\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  model: >-\n    One long-lived workspace bearer key, environment-separated by prefix. Simpler than the ATK API's\n    layered model because no browser or device ever holds a credential - the human signs on Tvarka's\n    own hosted page or in the Tvarka Sign mobile app, not in the integrator's client.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    header: 'Authorization: Bearer <key>'\n    sources: [openapi/tvarka-sign-api-openapi.yml]\n    description: >-\n      Keys are provisioned by Tvarka during onboarding and shown once. A tsk_live_ key acts on\n      production; a tsk_test_ key is the sandbox.\n\
  key_prefixes:\n  production: tsk_live_\n  sandbox: tsk_test_\nidentity_model:\n  binding: >-\n    The key acts as a NAMED WORKSPACE USER, not as an anonymous service principal. If that person's\n    role is revoked, or the workspace is suspended, the key stops working.\n  tenancy: >-\n    A tenant is a Tvarka entity with a Sign workspace; ceremonies are raised in that entity's name,\n    so the counterparty sees who is actually asking.\n  quoted_from: openapi/tvarka-sign-api-openapi.yml components.securitySchemes.bearerAuth.description\nmcp:\n  endpoint: https://sign-api.tvarka.pro/mcp\n  discovery_auth: none\n  invocation_auth: same bearer key\n  note: >-\n    tools/list and initialize answer anonymously (probed 2026-08-31, HTTP 200). Tool calls carry the\n    same Authorization: Bearer <key>. There is no OAuth: /.well-known/oauth-authorization-server and\n    /.well-known/oauth-protected-resource both 404 on sign-api.tvarka.pro.\nprovisioning:\n  request: info@tvarka.pro\n  note: A sandbox\
  \ tenant costs nothing and its key works before any funding.\nfailures:\n  - status: 401\n    applies_to: every operation\n  - status: 402\n    applies_to: [createSigning, createBatch, addSigner]\n    note: >-\n      Payment-required refusal. The problem body may carry recoveryUrl - a browser page for the\n      tenant's payment setup, explicitly NOT an API endpoint.\n  - status: 403\n    applies_to: [createSigning, simulateSigning]\n    note: simulateSigning is refused outright for a tsk_live_ key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/authentication/tvarka-sign-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Digital Signature
- eIDAS
- QES
- Lithuania
- OpenAPI
- eID
- Smart-ID
- Mobile-ID
- NFC
- Timestamping
- LTV
- Webhook
- Identity
- Trust Services
- GDPR
---
