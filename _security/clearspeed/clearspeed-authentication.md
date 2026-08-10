---
api_key_in:
- header
api_specs:
- filename: clearspeed-default-api-openapi.yml
  format: yaml
  label: Clearspeed Default API
  slug: clearspeed-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearspeed/refs/heads/main/openapi/clearspeed-default-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Clearspeed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clearspeed secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clearspeed
provider_slug: clearspeed
scheme_count: 1
schemes:
- applied_to: 'all 4 operations (each declares security: [{authorization: []}])'
  format: 'raw key value, no Bearer prefix — Authorization: <your-api-key>'
  in: header
  name: authorization
  parameter: Authorization
  sources:
  - openapi/clearspeed-integration-api-openapi.yml
  type: apiKey
slug: clearspeed-authentication
source_filename: clearspeed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://developer.clearspeed.com/api-keys\nderived_from: openapi/clearspeed-integration-api-openapi.yml\ndocs: https://developer.clearspeed.com/api-keys\napi: Clearspeed Integration API\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oidc: false\n  mutual_tls: false\nschemes:\n- name: authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'raw key value, no Bearer prefix — Authorization: <your-api-key>'\n  applied_to: 'all 4 operations (each declares security: [{authorization: []}])'\n  sources:\n  - openapi/clearspeed-integration-api-openapi.yml\nscoping:\n  unit: questionnaire\n  detail: >-\n    A key is bound to exactly one questionnaire. It is validated against the questionnaire\n    named by `project_uuid` in the participant request body, or by `questionnaire_id` in\n    the API-key management path. Cross-questionnaire use returns 403 \"API Key not\n    associated\
  \ with this Questionnaire\".\nscopes:\n- {scope: 'participant:write', allows: Create participants; update participant outcome,\n  in_spec_enum: true}\n- {scope: 'participant:read', allows: Read participant data, in_spec_enum: false, note: documented\n    on the portal but not enumerated in ApiKeyCreateRequest, and no read operation exists\n    in the published contract}\n- {scope: 'participant:delete', allows: Delete participants, in_spec_enum: false, note: documented\n    on the portal but not enumerated in ApiKeyCreateRequest, and no delete-participant\n    operation exists in the published contract}\n- {scope: 'apikey:write', allows: Create new API keys for the same questionnaire, in_spec_enum: true}\n- {scope: 'apikey:delete', allows: Delete API keys for the same questionnaire, in_spec_enum: true}\nscopes_note: >-\n  These are API-key permissions, not OAuth scopes — there is no oauth2 securityScheme on\n  the Integration API, so no scopes/ artifact is emitted. Two portal-documented\
  \ scopes\n  (participant:read, participant:delete) have no corresponding operation in the published\n  OpenAPI, which means either the contract is incomplete or those scopes govern an\n  unpublished surface.\nkey_lifecycle:\n  bootstrap: >-\n    The first key for a questionnaire must be created in the Clearspeed web app by a\n    questionnaire or tenant Admin (Integration page -> API Keys -> + Generate New).\n    Subsequent keys can be minted via createApiKey with the apikey:write scope.\n  visibility: >-\n    The full api_key value is returned only in the 201 response to createApiKey. There is\n    no list or read operation, so an unrecorded key value is unrecoverable — and delete\n    addresses the key by its raw value, so losing it also loses the ability to revoke it\n    through the API.\n  rotation: >-\n    Documented zero-downtime rotation: create a replacement with the same scopes, switch\n    the integration, verify, then delete the old key.\n  revocation: Immediate. A deleted\
  \ key returns 401 on the next request.\n  expiry: none documented\n  format: >-\n    Not specified in the docs. The OpenAPI create example shows a cs_live_ prefixed\n    placeholder; the delete example uses a bare 64-character hex value. The prefix is\n    therefore not guaranteed.\noutbound_authentication:\n  context: Clearspeed calling the customer's webhook endpoint\n  methods:\n  - {method: api-key, detail: 'Clearspeed sends a customer-supplied key value as a header\n      on every delivery'}\n  - {method: oauth2-client-credentials, detail: 'Clearspeed performs the client credentials\n      flow against a customer-supplied Token URL (Audience, Client ID, Client Secret)\n      before each delivery and sends an Authorization Bearer token'}\n  signature_verification: none\n  docs: https://developer.clearspeed.com/webhooks\n  note: >-\n    This is Clearspeed acting as an OAuth CLIENT against the customer. It is not\n    authentication to the Clearspeed API and does not make the Integration\
  \ API an OAuth API.\nother_auth_surfaces:\n- surface: developer portal MCP server\n  url: https://developer.clearspeed.com/mcp\n  scheme: OAuth 2.1 bearer (RFC 9728 protected resource)\n  issuer: https://auth.cloud.redocly.com\n  note: >-\n    Redocly Reunite portal identity protecting the documentation MCP server. Unrelated to\n    Integration API authentication. See mcp/clearspeed-mcp.yml.\ngaps:\n- No IP allowlisting documented.\n- No mTLS option.\n- No key expiry or last-used telemetry.\n- No list-keys operation, so key inventory must be maintained client-side.\n- No rate limits tied to a key.\nx-evidence:\n  fetched: '2026-08-04'\n  sources:\n  - {url: 'https://developer.clearspeed.com/api-keys', http_status: 200}\n  - {url: 'https://developer.clearspeed.com/webhooks', http_status: 200}\ncross_links:\n  conventions: conventions/clearspeed-conventions.yml\n  errors: errors/clearspeed-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearspeed/refs/heads/main/authentication/clearspeed-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Risk Assessment
- Fraud Detection
- Voice Analytics
- Artificial Intelligence
- Insurance
- Identity Verification
- Screening
- Security
---
