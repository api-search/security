---
api_key_in:
- header
api_specs:
- filename: vehicles-dev-api-admin-api-openapi.yml
  format: yaml
  label: Vehicles.dev Admin API
  slug: vehicles-dev-api-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicles-dev-api/refs/heads/main/openapi/vehicles-dev-api-admin-api-openapi.yml
- filename: vehicles-dev-api-billing-api-openapi.yml
  format: yaml
  label: Vehicles.dev Billing API
  slug: vehicles-dev-api-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicles-dev-api/refs/heads/main/openapi/vehicles-dev-api-billing-api-openapi.yml
- filename: vehicles-dev-api-control-api-openapi.yml
  format: yaml
  label: Vehicles.dev Control API
  slug: vehicles-dev-api-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicles-dev-api/refs/heads/main/openapi/vehicles-dev-api-control-api-openapi.yml
- filename: vehicles-dev-api-data-api-openapi.yml
  format: yaml
  label: Vehicles.dev Data API
  slug: vehicles-dev-api-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicles-dev-api/refs/heads/main/openapi/vehicles-dev-api-data-api-openapi.yml
- filename: vehicles-dev-api-employment-api-openapi.yml
  format: yaml
  label: Vehicles.dev Employment API
  slug: vehicles-dev-api-employment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicles-dev-api/refs/heads/main/openapi/vehicles-dev-api-employment-api-openapi.yml
- filename: vehicles-dev-api-operations-api-openapi.yml
  format: yaml
  label: Vehicles.dev Operations API
  slug: vehicles-dev-api-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicles-dev-api/refs/heads/main/openapi/vehicles-dev-api-operations-api-openapi.yml
- filename: vehicles-dev-api-operator-api-openapi.yml
  format: yaml
  label: Vehicles.dev Operator API
  slug: vehicles-dev-api-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicles-dev-api/refs/heads/main/openapi/vehicles-dev-api-operator-api-openapi.yml
- filename: vehicles-dev-api-reports-api-openapi.yml
  format: yaml
  label: Vehicles.dev Reports API
  slug: vehicles-dev-api-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicles-dev-api/refs/heads/main/openapi/vehicles-dev-api-reports-api-openapi.yml
- filename: vehicles-dev-api-vehicles-api-openapi.yml
  format: yaml
  label: Vehicles.dev Vehicles API
  slug: vehicles-dev-api-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicles-dev-api/refs/heads/main/openapi/vehicles-dev-api-vehicles-api-openapi.yml
- filename: vehicles-dev-api-webhooks-api-openapi.yml
  format: yaml
  label: Vehicles.dev Webhooks API
  slug: vehicles-dev-api-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicles-dev-api/refs/heads/main/openapi/vehicles-dev-api-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Vehicles Dev Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vehicles.dev secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vehicles.dev
provider_slug: vehicles-dev-api
scheme_count: 2
schemes:
- applies_to:
  - /v1/vehicles/*
  - /v1/employment/*
  audience: data plane
  bearerFormat: Product API key
  header: Authorization
  name: apiKeyBearer
  operations: 16
  prefix: vdev_
  scheme: bearer
  sources:
  - openapi/vehicles-dev-api-vehicles-api-openapi.yml
  - openapi/vehicles-dev-api-data-api-openapi.yml
  - openapi/vehicles-dev-api-employment-api-openapi.yml
  - openapi/vehicles-dev-api-reports-api-openapi.yml
  type: http
- applies_to:
  - /v1/control/*
  - /v1/ops/*
  audience: dashboard control plane and operator plane
  bearerFormat: WorkOS access token
  header: Authorization
  identity_provider: WorkOS
  identity_provider_note: Inferred from the scheme's own bearerFormat, "WorkOS access token", declared by the provider in its own spec. No authorization-server metadata is published — /.well-known/oauth-authorization-server and /.well-known/openid-configuration both 404 — so the token issuance flow is not machine-discoverable.
  name: workosBearer
  operations: 41
  scheme: bearer
  sources:
  - openapi/vehicles-dev-api-control-api-openapi.yml
  - openapi/vehicles-dev-api-operator-api-openapi.yml
  - openapi/vehicles-dev-api-admin-api-openapi.yml
  - openapi/vehicles-dev-api-billing-api-openapi.yml
  type: http
slug: vehicles-dev-api-authentication
source_filename: vehicles-dev-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: searched\nsource: https://vehicles.dev/docs#authentication\ndocs: https://vehicles.dev/docs#authentication\nderived_from: openapi/_original/vehicles-dev-api-openapi.json\nnote: >-\n  Upgraded from the mechanical derive, which reported only apiKeyBearer. The contract declares TWO\n  bearer schemes and they gate different planes: apiKeyBearer (a vdev_ product key) on the data plane,\n  workosBearer (a WorkOS dashboard session token) on the control and operator planes. Presenting a\n  vdev_ key to a control-plane route returns 401 invalid_credential.\nsummary:\n  types: [http]\n  schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  planes: 2\nschemes:\n  - name: apiKeyBearer\n    type: http\n    scheme: bearer\n    bearerFormat: Product API key\n    header: Authorization\n    prefix: vdev_\n    audience: data plane\n    applies_to:\n      - /v1/vehicles/*\n      - /v1/employment/*\n    operations: 16\n    sources:\n      - openapi/vehicles-dev-api-vehicles-api-openapi.yml\n\
  \      - openapi/vehicles-dev-api-data-api-openapi.yml\n      - openapi/vehicles-dev-api-employment-api-openapi.yml\n      - openapi/vehicles-dev-api-reports-api-openapi.yml\n  - name: workosBearer\n    type: http\n    scheme: bearer\n    bearerFormat: WorkOS access token\n    header: Authorization\n    audience: dashboard control plane and operator plane\n    applies_to:\n      - /v1/control/*\n      - /v1/ops/*\n    operations: 41\n    identity_provider: WorkOS\n    identity_provider_note: >-\n      Inferred from the scheme's own bearerFormat, \"WorkOS access token\", declared by the provider in\n      its own spec. No authorization-server metadata is published — /.well-known/oauth-authorization-server\n      and /.well-known/openid-configuration both 404 — so the token issuance flow is not machine-discoverable.\n    sources:\n      - openapi/vehicles-dev-api-control-api-openapi.yml\n      - openapi/vehicles-dev-api-operator-api-openapi.yml\n      - openapi/vehicles-dev-api-admin-api-openapi.yml\n\
  \      - openapi/vehicles-dev-api-billing-api-openapi.yml\nunauthenticated_operations:\n  - {operation: getApiLiveness, path: /health/live}\n  - {operation: getApiReadiness, path: /health/ready}\n  - {operation: getOpenApiDocument, path: /openapi.json}\n  - operation: receivePaymentWebhook\n    path: '/webhooks/payments/{product}'\n    note: signature-verified inbound processor webhook\nusage:\n  header_format: 'Authorization: Bearer $VEHICLES_API_KEY'\n  scheme_token_case_sensitive: true\n  rejected_forms:\n    - {form: 'lowercase \"bearer\"', result: 401 invalid_credential}\n    - {form: double space after scheme, result: 401 invalid_credential}\n    - {form: query-string key, result: unsupported}\n    - {form: HTTP basic, result: unsupported}\n    - {form: Cookie header, result: 401 cookie_credentials_rejected}\nkey_management:\n  mint: dashboard API keys panel (https://vehicles.dev/dashboard)\n  api: 'POST /v1/control/api-keys (createControlApiKey) — requires a WorkOS session token,\
  \ not an API key'\n  revoke_api: 'DELETE /v1/control/api-keys/{id} (revokeControlApiKey)'\n  list_api: 'GET /v1/control/api-keys (listControlApiKeys)'\n  secret_visibility: displayed exactly once at creation and never recoverable\n  storage: provider stores only a hash and the last four characters\n  rotation: create-then-revoke; revocation takes effect immediately\n  product_scoping: >-\n    Keys are scoped to a single product. A key minted for another product on the same platform returns\n    401 invalid_credential.\n  enforcement_scope: >-\n    Rate limits and credit balances are enforced per account, not per key — splitting traffic across\n    several keys does not raise the throughput ceiling.\npermissions:\n  model: named permissions on machine keys (documented in prose, not in the contract)\n  note: >-\n    Not OAuth scopes — there is no oauth2 securityScheme and no scopes map in the OpenAPI, so no\n    scopes/ artifact is emitted. These permission strings appear only in the vehicle-history-report\n\
  \    section of the docs.\n  observed:\n    - {name: 'reports:order', requirement: 'Creating a history report, and explicitly retrying a durable submitting job, on the machine route'}\n    - {name: 'reports:read', requirement: Polling report status and reading the report result}\n    - {name: 'billing:write', requirement: The dashboard route for retrying a history-report submission}\nordering:\n  note: >-\n    Authentication runs before schema validation. A request that is both unauthenticated and malformed\n    returns 401, never 400.\ntransport_security:\n  https_required: true\n  tls_version_observed: TLSv1.3\n  hsts: false\n  see: security/vehicles-dev-api-domain-security.yml\noperational_guidance:\n  - Keep the key server-side; the API is not browser-callable and rejects any request carrying an Origin header.\n  - Never send a full key to support; redact to the last four characters.\n  - Authorization and Cookie headers are redacted from provider logs, so quote x-request-id instead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vehicles-dev-api/refs/heads/main/authentication/vehicles-dev-api-authentication.yml
summary_line: http · 2 schemes
tags:
- Automotive
- Vehicle Data
- VIN Decoding
- Vehicle Valuation
- Market Value
- Vehicle Listings
- Recalls
- NHTSA
- vPIC
- Vehicle Specifications
- Depreciation
- Ownership Costs
- Job
- Labor Market Data
- REST
- OpenAPI
- Vehicle Safety
- Car Listings
- Marketplace
- Pricing
- Cost of Ownership
- Vehicle Images
- MCP
- Agent Tools
- Machine-Learning
---
