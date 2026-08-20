---
api_key_in:
- header
api_specs:
- filename: intelycare-external-scheduling-openapi.yml
  format: yaml
  label: IntelyCare External Scheduling API
  slug: intelycare-external-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelycare/refs/heads/main/openapi/intelycare-external-scheduling-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Intelycare Authentication
name_suffix: Authentication
oauth_flows: []
overview: IntelyCare secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: IntelyCare
provider_slug: intelycare
scheme_count: 2
schemes:
- applies_to:
  - shift_create_api_v1
  - shift_update_api_v1
  - shift_delete_api_v1
  - timecard_create_api_v1
  - update_timecard_api_v1
  - check_in_out_api_v1
  description: API key issued to a specific client. This can only be used to access data within the client scope. "API Keys are tied to individual clients and cannot be used outside their provided scope."
  direction: inbound
  example_shape: uuid v4
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/intelycare-external-scheduling-openapi.yml
  type: apiKey
- actual_mechanism: HMAC-SHA256 hex digest of the body payload, computed with the webhook secret
  applies_to:
  - shift_accept_webhook_v1
  - shift_release_webhook_v1
  description: The hash signature of the payload. IntelyCare webhooks use a HMAC hex digest (SHA256) to compute the signature of the body payload with the webhook secret. Verify in constant time before processing a webhook; it is the only authentication on the callback.
  direction: outbound
  in: header
  name: HMACSignature
  parameter: X-Signature-IC
  sources:
  - openapi/intelycare-external-scheduling-openapi.yml
  type: apiKey
slug: intelycare-authentication
source_filename: intelycare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/intelycare-external-scheduling-openapi.yml\ndocs: https://apidocs.intelycare.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oidc: false\n  mutual_tls: false\n  note: >-\n    Two apiKey-typed schemes serve two different directions. ApiKeyAuth (X-API-KEY) authenticates\n    the CLIENT calling IntelyCare on all six REST operations. HMACSignature (X-Signature-IC)\n    authenticates INTELYCARE calling the client's webhook receiver — it is modelled as an apiKey\n    scheme in the OpenAPI, but it is not a static key: it is an HMAC hex digest (SHA256) of the\n    body payload computed with the webhook secret, and must be recomputed and compared per\n    request.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  direction: inbound\n  description: >-\n    API key issued to a specific client. This can only be used to access data within the client\n  \
  \  scope. \"API Keys are tied to individual clients and cannot be used outside their provided\n    scope.\"\n  example_shape: uuid v4\n  applies_to:\n  - shift_create_api_v1\n  - shift_update_api_v1\n  - shift_delete_api_v1\n  - timecard_create_api_v1\n  - update_timecard_api_v1\n  - check_in_out_api_v1\n  sources:\n  - openapi/intelycare-external-scheduling-openapi.yml\n- name: HMACSignature\n  type: apiKey\n  in: header\n  parameter: X-Signature-IC\n  direction: outbound\n  actual_mechanism: HMAC-SHA256 hex digest of the body payload, computed with the webhook secret\n  description: >-\n    The hash signature of the payload. IntelyCare webhooks use a HMAC hex digest (SHA256) to\n    compute the signature of the body payload with the webhook secret. Verify in constant time\n    before processing a webhook; it is the only authentication on the callback.\n  applies_to:\n  - shift_accept_webhook_v1\n  - shift_release_webhook_v1\n  sources:\n  - openapi/intelycare-external-scheduling-openapi.yml\n\
  companion_headers:\n- name: X-CLIENT-ID\n  required: true\n  description: >-\n    IntelyCare's unique identifier of the client. Required on all six REST operations alongside\n    X-API-KEY. It is declared as a required parameter on every operation but is NOT declared as a\n    securityScheme, so a spec-driven client generator will not treat it as a credential.\n  applies_to:\n  - shift_create_api_v1\n  - shift_update_api_v1\n  - shift_delete_api_v1\n  - timecard_create_api_v1\n  - update_timecard_api_v1\n  - check_in_out_api_v1\nkey_management:\n  self_serve: false\n  rotation_policy: not published\n  provisioning: Keys are issued per client by IntelyCare; contact apisupport@intelycare.com\n  scopes: none — the key is scoped to a client, not to permissions\n  expiry: not published\nfailure_mode:\n  status: 401\n  body: {message: Unauthorized}\n  header: WWW_Authenticate\n  header_note: >-\n    Declared with an underscore in the published spec; the RFC 9110 header is WWW-Authenticate.\n\
  gaps:\n- No OAuth 2.0 or OpenID Connect; /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server return 404 (www) / 403 (api host).\n- No scope or permission model — a key is all-or-nothing inside its client scope.\n- X-CLIENT-ID is a required credential-adjacent header but is not modelled as a securityScheme.\n- No documented key rotation, expiry, or revocation process.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intelycare/refs/heads/main/authentication/intelycare-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Healthcare
- Healthcare Staffing
- Nursing
- Workforce Management
- Scheduling
- Shift Management
- Timekeeping
- Marketplace
- Webhook
- Per Diem
- Credentialing
- Post-Acute Care
---
