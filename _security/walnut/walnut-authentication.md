---
api_key_in: []
auth_types: []
description: 'Walnut authenticates the Customer Data API with a single static API key sent in the x-api-key request header. There is no OAuth, no OIDC, no bearer token and no self-service key management: keys are provisioned out-of-band by a Walnut account representative, shown once, and cannot be rotated or recovered by the customer. Webhook deliveries are authenticated in the opposite direction with an HMAC-SHA256 signature. Human access to the Walnut application is separate and supports SAML SSO with SCIM provisioning on the Accelerate and Scale plans.'
kind: authentication
layout: security
method: searched
name: Walnut Authentication
name_suffix: Authentication
oauth_flows: []
overview: Walnut declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Walnut
provider_slug: walnut
scheme_count: 0
schemes: []
slug: walnut-authentication
source_filename: walnut-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Walnut Authentication\ndescription: >-\n  Walnut authenticates the Customer Data API with a single static API key sent in the x-api-key\n  request header. There is no OAuth, no OIDC, no bearer token and no self-service key management:\n  keys are provisioned out-of-band by a Walnut account representative, shown once, and cannot be\n  rotated or recovered by the customer. Webhook deliveries are authenticated in the opposite\n  direction with an HMAC-SHA256 signature. Human access to the Walnut application is separate and\n  supports SAML SSO with SCIM provisioning on the Accelerate and Scale plans.\ngenerated: '2026-08-13'\nmethod: searched\nsource: https://help.walnut.io/help/api/customer-data-api\ndocs:\n  - https://help.walnut.io/help/api/customer-data-api\n  - https://help.walnut.io/help/api/quick-start\n  - https://help.walnut.io/help/api/webhooks\n  - https://help.walnut.io/help/account/users/sso-and-scim\n\napi: Walnut Customer Data API\nbase_url: https://customer-api.teamwalnut.com\n\
  \nsecurity_schemes:\n  - id: apiKeyHeader\n    type: apiKey\n    in: header\n    name: x-api-key\n    description: >-\n      Static, long-lived API key. Required on every endpoint except GET /health. Walnut's\n      quick-start documents that keys are prefixed wlt_.\n    key_prefix: wlt_\n    applied_to: all endpoints except /health\n    source: https://help.walnut.io/help/api/customer-data-api\n    example_header: \"x-api-key: YOUR_API_KEY\"\n  - id: hmacWebhookSignature\n    type: http\n    scheme: hmac\n    direction: inbound-to-customer\n    header: X-Walnut-Signature\n    algorithm: HMAC-SHA256\n    encoding: lowercase hexadecimal\n    signed_payload: the raw request body, exactly as received\n    description: >-\n      Optional but strongly recommended by Walnut. Configured per webhook in Settings >\n      Webhooks; the shared signing key can be reset from the same screen, which immediately\n      invalidates the previous key.\n    source: https://help.walnut.io/help/api/webhooks\n\
  \noauth2: false\nopenid_connect: false\nmutual_tls: false\nbearer_token: false\n\nkey_lifecycle:\n  self_service_issuance: false\n  self_service_rotation: false\n  recoverable: false\n  issued_by: Walnut account representative\n  shown_once: true\n  revocation: Request through the Walnut account team.\n  propagation_delay: >-\n    Up to 5 minutes. Walnut documents that API key changes, including revocations, may take up\n    to five minutes to take effect because authorization decisions are cached.\n  notes:\n    - >-\n      \"Your API key is provided once by the Walnut team and cannot be recovered if lost.\"\n      Losing a key requires contacting an account representative for a replacement.\n    - >-\n      There is no scoping mechanism. A key is account-wide and read-only; the API exposes no\n      write operations, so a key cannot mutate data.\n\nunauthenticated_surface:\n  - path: /health\n    method: GET\n    response: '{ \"status\": \"ok\" }'\n    note: >-\n      The only endpoint\
  \ that accepts anonymous requests. Verified live 2026-08-13:\n      GET https://customer-api.teamwalnut.com/health returned HTTP 200 {\"status\": \"ok\"}.\n\nfailure_modes:\n  - status: 401\n    meaning: Unauthorized\n    cause: Missing or invalid API key.\n    remediation: >-\n      Send the key in the x-api-key header, not Authorization. Verified live 2026-08-13:\n      an unauthenticated GET /demo-sessions returns 401 {\"message\":\"Unauthorized\"}.\n  - status: 403\n    meaning: Forbidden\n    cause: The API key is incorrect or no longer active.\n    remediation: Confirm the key with the Walnut account team; allow up to 5 minutes after a key change.\n\napplication_authentication:\n  description: >-\n    Authentication for humans signing in to the Walnut application at app.teamwalnut.com. This\n    is a separate surface from the Customer Data API and does not issue API credentials.\n  methods:\n    - name: Email and password\n      available: all plans\n    - name: SSO (SAML)\n    \
  \  available: Accelerate and Scale\n      source: https://www.walnut.io/pricing\n    - name: SCIM provisioning\n      available: Accelerate and Scale\n      source: https://www.walnut.io/pricing\n  docs: https://help.walnut.io/help/account/users/sso-and-scim\n  roles:\n    - Account Owner\n    - Admin\n    - Editor\n    - Presenter\n    - Collaborator\n  roles_docs: https://help.walnut.io/help/account/users/roles-and-permissions\n\ngaps:\n  - No OAuth 2.0 or OIDC flow for third-party or delegated access.\n  - No self-service key creation, rotation, or revocation, and no key-management UI.\n  - No per-key scoping or least-privilege model; a key is account-wide.\n  - >-\n    No published /.well-known/oauth-authorization-server or /.well-known/openid-configuration\n    on any Walnut host (see well-known/walnut-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walnut/refs/heads/main/authentication/walnut-authentication.yml
summary_line: 0 schemes
tags:
- Sales Demo
- Interactive Demos
- Product Demos
- Sales Enablement
- Demo Analytics
- Go-to-Market
- AI-Powered
- Webhooks
- MCP
- Analytics
---
