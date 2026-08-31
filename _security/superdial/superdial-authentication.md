---
api_key_in:
- header
api_specs:
- filename: superdial-api-openapi.yml
  format: yaml
  label: SuperDial API
  slug: superdial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superdial/refs/heads/main/openapi/superdial-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Superdial Authentication
name_suffix: Authentication
oauth_flows: []
overview: SuperDial secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SuperDial
provider_slug: superdial
scheme_count: 3
schemes:
- description: Your SuperDial API key
  in: header
  name: apiKey
  parameter: Robodialer-API-Key
  role: Identifies the account. Sent to GET /v1/auth only.
  sources:
  - openapi/superdial-api-openapi.yml
  type: apiKey
- description: Your SuperDial API secret
  in: header
  name: apiSecret
  parameter: Robodialer-API-Secret
  role: Authenticates the request. Sent to GET /v1/auth only.
  sources:
  - openapi/superdial-api-openapi.yml
  type: apiKey
- description: Bearer token obtained from the /v1/auth endpoint
  name: bearerAuth
  role: Authorizes every other operation. Obtained from GET /v1/auth, lives 1 hour.
  scheme: bearer
  sources:
  - openapi/superdial-api-openapi.yml
  type: http
slug: superdial-authentication
source_filename: superdial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://docs.superdial.com/api-reference/authentication/authenticate-and-get-token\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Robodialer-API-Key\n  description: Your SuperDial API key\n  sources:\n  - openapi/superdial-api-openapi.yml\n  role: Identifies the account. Sent to GET /v1/auth only.\n- name: apiSecret\n  type: apiKey\n  in: header\n  parameter: Robodialer-API-Secret\n  description: Your SuperDial API secret\n  sources:\n  - openapi/superdial-api-openapi.yml\n  role: Authenticates the request. Sent to GET /v1/auth only.\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from the /v1/auth endpoint\n  sources:\n  - openapi/superdial-api-openapi.yml\n  role: Authorizes every other operation. Obtained from GET /v1/auth, lives 1 hour.\ndocs: https://docs.superdial.com/guides/creating-a-request#authentication\n\
  model:\n  style: key-secret-exchange-for-bearer-token\n  description: 'Two distinct values are issued together: the API KEY identifies the account, the API SECRET\n    authenticates the request. Both are sent as headers to GET /v1/auth, which returns a short-lived bearer\n    token. Every other operation takes Authorization: Bearer <token>.'\n  token_lifetime: 1 hour\n  token_endpoint: GET /v1/auth\n  oauth2: false\n  scopes: null\n  mtls: false\n  note: No OAuth 2.0 and no scope surface, so no scopes/ artifact is emitted — the model is account-wide\n    bearer access rather than delegated, scoped authorization.\ncredential_environments:\n- name: production\n  provisioning: account team\n  note: Also the default webhook signing secret when no separate webhook secret is set.\n- name: sandbox\n  provisioning: account team, on request\n  note: A distinct key/secret pair. Authenticating with it routes every request through the sandbox path\n    automatically — there is no per-request flag.\n\
  webhook_verification:\n  header: X-Webhook-Signature\n  algorithm: HMAC-SHA256\n  encoding: bare 64-character lowercase hex digest\n  secret: The account webhook secret if configured, otherwise the PRODUCTION API key — including for sandbox\n    webhooks.\n  gotcha: Verifying a sandbox webhook with the sandbox API key will fail. The production-side secret signs\n    both.\nnotes:\n- The spec declares three securitySchemes but no top-level `security` requirement and no per-operation\n  security block, so the OpenAPI alone does not state which scheme applies where. That mapping comes from\n  the docs and is recorded above.\n- 'No self-serve signup: credentials are provisioned by the SuperDial account team. An agent cannot obtain\n  access programmatically.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superdial/refs/heads/main/authentication/superdial-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Healthcare
- Revenue Cycle Management
- Voice AI
- Insurance
- Artificial Intelligence
- Claims
- Prior Authorization
- Benefits Verification
- Automation
---
