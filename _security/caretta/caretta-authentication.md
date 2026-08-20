---
api_key_in: []
auth_types:
- oauth2
- hmac
description: ''
kind: authentication
layout: security
method: searched
name: Caretta Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Caretta secures its APIs with oauth2 and hmac across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Caretta
provider_slug: caretta
scheme_count: 3
schemes:
- applies_to: https://gateway.caretta.app/mcp
  authorization_model: Tokens are user-delegated. The server follows the signed-in user's existing Caretta permissions and cannot return calls the user could not otherwise see.
  authorization_servers:
  - https://ztejbfpbhxgwecvxngtf.supabase.co/auth/v1
  bearer_methods_supported:
  - header
  browser_based_consent: true
  challenge_observed: 'WWW-Authenticate: Bearer realm="caretta-mcp", resource_metadata="https://gateway.caretta.app/.well-known/oauth-protected-resource/mcp"'
  dynamic_client_registration: true
  flow: authorizationCode
  metadata_spec: RFC 9728
  name: MCP OAuth
  protected_resource_metadata: https://gateway.caretta.app/.well-known/oauth-protected-resource
  revocation: Settings -> Caretta MCP -> Unauthorise, per client.
  scopes:
  - calls:read
  - todos:read
  - todos:write
  scopes_artifact: scopes/caretta-scopes.yml
  sources:
  - https://www.caretta.so/docs/caretta-mcp
  surface: inbound
  token_type: Bearer
  type: oauth2
- algorithm: HMAC-SHA256
  applies_to: customer HTTPS endpoints
  name: Webhook signature
  reference_implementation: Node.js verifier published in the docs using crypto.createHmac and crypto.timingSafeEqual.
  replay_window_seconds: 300
  secret_distribution: per-endpoint signing secret, displayed once at creation
  secret_rotation: supported in Settings -> Webhooks; previous secret invalidated immediately
  signature_format: v1=<hex digest>
  signature_header: X-Caretta-Signature
  signed_payload: '{timestamp}.{raw request body}'
  sources:
  - https://www.caretta.so/docs/webhooks
  surface: outbound
  timestamp_header: X-Caretta-Timestamp
  type: hmac
- admin_approval: may be required by the customer's Zoom account policy
  applies_to: Zoom API on behalf of the connecting user
  flow: authorizationCode
  least_privilege_claim: Provider states Caretta does not request permission to read the Zoom profile, list existing meetings, access recordings, read transcripts, or join meetings. One permission only.
  name: Zoom OAuth (third-party, outbound)
  revocation: Caretta Settings -> Integrations -> Disconnect, and/or Zoom Marketplace -> Added Apps -> Remove
  scopes_requested:
  - meeting:write:meeting
  sources:
  - https://www.caretta.so/docs/zoom
  surface: outbound-integration
  token_storage: access and refresh tokens stored by Caretta to keep the connection working
  type: oauth2
slug: caretta-authentication
source_filename: caretta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.caretta.so/docs/caretta-mcp\ndocs:\n- https://www.caretta.so/docs/caretta-mcp\n- https://www.caretta.so/docs/webhooks\n- https://www.caretta.so/docs/zoom\nnote: >-\n  Derived by hand, not by derive-authentication.py: Caretta publishes no OpenAPI\n  document, so there are no securitySchemes to aggregate. Everything below is\n  transcribed from the provider's published docs and from live probes of the\n  gateway host.\n\nsummary:\n  types: [oauth2, hmac]\n  api_key_issued: false\n  api_key_note: >-\n    Provider states verbatim: \"You do not need to create an API key.\" There is no\n    key-issuance surface at all.\n  oauth2_flows: [authorizationCode]\n  inbound_auth: oauth2 bearer (MCP only)\n  outbound_auth: HMAC-SHA256 request signing (webhooks)\n\nschemes:\n- name: MCP OAuth\n  type: oauth2\n  surface: inbound\n  applies_to: https://gateway.caretta.app/mcp\n  flow: authorizationCode\n  token_type: Bearer\n  bearer_methods_supported:\
  \ [header]\n  browser_based_consent: true\n  dynamic_client_registration: true\n  protected_resource_metadata: https://gateway.caretta.app/.well-known/oauth-protected-resource\n  metadata_spec: RFC 9728\n  authorization_servers: [https://ztejbfpbhxgwecvxngtf.supabase.co/auth/v1]\n  scopes: [calls:read, todos:read, todos:write]\n  scopes_artifact: scopes/caretta-scopes.yml\n  challenge_observed: >-\n    WWW-Authenticate: Bearer realm=\"caretta-mcp\",\n    resource_metadata=\"https://gateway.caretta.app/.well-known/oauth-protected-resource/mcp\"\n  authorization_model: >-\n    Tokens are user-delegated. The server follows the signed-in user's existing\n    Caretta permissions and cannot return calls the user could not otherwise see.\n  revocation: Settings -> Caretta MCP -> Unauthorise, per client.\n  sources: [https://www.caretta.so/docs/caretta-mcp]\n\n- name: Webhook signature\n  type: hmac\n  surface: outbound\n  applies_to: customer HTTPS endpoints\n  algorithm: HMAC-SHA256\n  signed_payload:\
  \ '{timestamp}.{raw request body}'\n  signature_header: X-Caretta-Signature\n  signature_format: 'v1=<hex digest>'\n  timestamp_header: X-Caretta-Timestamp\n  replay_window_seconds: 300\n  secret_distribution: per-endpoint signing secret, displayed once at creation\n  secret_rotation: supported in Settings -> Webhooks; previous secret invalidated immediately\n  reference_implementation: >-\n    Node.js verifier published in the docs using crypto.createHmac and\n    crypto.timingSafeEqual.\n  sources: [https://www.caretta.so/docs/webhooks]\n\n- name: Zoom OAuth (third-party, outbound)\n  type: oauth2\n  surface: outbound-integration\n  applies_to: Zoom API on behalf of the connecting user\n  flow: authorizationCode\n  scopes_requested: [meeting:write:meeting]\n  token_storage: access and refresh tokens stored by Caretta to keep the connection working\n  least_privilege_claim: >-\n    Provider states Caretta does not request permission to read the Zoom profile,\n    list existing meetings,\
  \ access recordings, read transcripts, or join\n    meetings. One permission only.\n  admin_approval: may be required by the customer's Zoom account policy\n  revocation: Caretta Settings -> Integrations -> Disconnect, and/or Zoom Marketplace -> Added Apps -> Remove\n  sources: [https://www.caretta.so/docs/zoom]\n\nx-evidence:\n- url: https://gateway.caretta.app/mcp\n  http_status: 401\n  fetched: '2026-08-13'\n  note: anonymous POST returns the bearer challenge above\n- url: https://gateway.caretta.app/.well-known/oauth-protected-resource\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://www.caretta.so/docs/caretta-mcp\n  http_status: 200\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caretta/refs/heads/main/authentication/caretta-authentication.yml
summary_line: oauth2/hmac · 3 schemes
tags:
- Company
- Artificial Intelligence
- Sales
- Sales Intelligence
- Real-Time
- Conversation Intelligence
- Revenue Operations
- Y Combinator
- MCP
- Webhook
- Agents
---
