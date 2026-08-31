---
api_key_in:
- header
api_specs:
- filename: justt-chargebacks-api-openapi.yml
  format: yaml
  label: Justt Chargebacks API
  slug: justt-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-chargebacks-api-openapi.yml
- filename: justt-data-subjects-api-openapi.yml
  format: yaml
  label: Justt Data Subjects API
  slug: justt-data-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-data-subjects-api-openapi.yml
- filename: justt-evidence-api-openapi.yml
  format: yaml
  label: Justt Evidence API
  slug: justt-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-evidence-api-openapi.yml
- filename: justt-files-api-openapi.yml
  format: yaml
  label: Justt Files API
  slug: justt-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-files-api-openapi.yml
- filename: justt-integrations-api-openapi.yml
  format: yaml
  label: Justt Integrations API
  slug: justt-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-integrations-api-openapi.yml
- filename: justt-merchants-api-openapi.yml
  format: yaml
  label: Justt Merchants API
  slug: justt-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-merchants-api-openapi.yml
- filename: justt-pre-chargeback-alerts-api-openapi.yml
  format: yaml
  label: Justt Pre-chargeback Alerts API
  slug: justt-pre-chargeback-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-pre-chargeback-alerts-api-openapi.yml
- filename: justt-sandbox-api-openapi.yml
  format: yaml
  label: Justt Sandbox API
  slug: justt-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-sandbox-api-openapi.yml
- filename: justt-transactions-api-openapi.yml
  format: yaml
  label: Justt Transactions API
  slug: justt-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-transactions-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Justt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Justt secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Justt
provider_slug: justt
scheme_count: 3
schemes:
- applies_to: Justt REST API, Pre-Chargeback Alerts API
  bearerFormat: JWT
  docs: https://developers.justt.ai/docs/authentication
  environment_specific: true
  format: 'Authorization: Bearer <api-key>'
  in: header
  issuance: https://app.justt.ai/connect-psp/integration/api-integration
  name: bearer
  note: 'The spec declares bearerFormat: JWT, but the documentation consistently calls the credential an "API key" obtained from the hub rather than a token minted by a login flow. Treat it as a long-lived static bearer credential. Justt states the keys "come with a significant level of privilege" and warns against committing them.'
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/justt-rest-api-openapi-original.json
  - openapi/justt-pre-chargeback-alerts-openapi-original.json
  type: http
- algorithm: HMAC-SHA256
  applies_to: inbound webhooks (Justt -> merchant)
  direction: inbound
  docs: https://developers.justt.ai/docs/signature-verification
  in: header
  name: svix-signature
  note: 'This scheme secures the reverse direction: it authenticates Justt to the merchant''s endpoint, not the merchant to Justt. The documented header triple is webhook-id / webhook-timestamp / webhook-signature (Standard Webhooks); the spec names the Svix header. Verify against the raw request body with a 5-minute timestamp tolerance.'
  parameter: svix-signature
  sources:
  - asyncapi/justt-webhook-events-openapi-original.json
  type: apiKey
- applies_to: the MCP endpoint at justt.ai/wp-json/mcp/mcp-oauth-server
  authorization_endpoint: https://justt.ai/oauth/authorize
  authorization_server: https://justt.ai
  grant_types:
  - authorization_code
  - refresh_token
  name: mcp-oauth
  note: Discovered by probe, not documented. This OAuth surface belongs to the MCP endpoint on the WordPress marketing host and has NOTHING to do with the chargeback API, which never uses OAuth. Recorded so an agent does not attempt an OAuth dance against api.justt.ai.
  pkce: S256
  revocation_endpoint: https://justt.ai/oauth/revoke
  scopes:
  - mcp
  sources:
  - well-known/justt-oauth-authorization-server.json
  - well-known/justt-oauth-protected-resource.json
  token_endpoint: https://justt.ai/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: justt-authentication
source_filename: justt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: >-\n  https://developers.justt.ai/docs/authentication,\n  openapi/justt-rest-api-openapi-original.json,\n  openapi/justt-pre-chargeback-alerts-openapi-original.json,\n  asyncapi/justt-webhook-events-openapi-original.json,\n  https://justt.ai/.well-known/oauth-authorization-server\ndocs: https://developers.justt.ai/docs/authentication\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  primary: bearer API key in the Authorization header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer <api-key>'\n  applies_to: Justt REST API, Pre-Chargeback Alerts API\n  issuance: https://app.justt.ai/connect-psp/integration/api-integration\n  environment_specific: true\n  docs: https://developers.justt.ai/docs/authentication\n  sources:\n  - openapi/justt-rest-api-openapi-original.json\n  - openapi/justt-pre-chargeback-alerts-openapi-original.json\n\
  \  note: >-\n    The spec declares bearerFormat: JWT, but the documentation consistently calls\n    the credential an \"API key\" obtained from the hub rather than a token minted by\n    a login flow. Treat it as a long-lived static bearer credential. Justt states\n    the keys \"come with a significant level of privilege\" and warns against\n    committing them.\n- name: svix-signature\n  type: apiKey\n  in: header\n  parameter: svix-signature\n  applies_to: inbound webhooks (Justt -> merchant)\n  direction: inbound\n  algorithm: HMAC-SHA256\n  sources:\n  - asyncapi/justt-webhook-events-openapi-original.json\n  note: >-\n    This scheme secures the reverse direction: it authenticates Justt to the\n    merchant's endpoint, not the merchant to Justt. The documented header triple is\n    webhook-id / webhook-timestamp / webhook-signature (Standard Webhooks); the\n    spec names the Svix header. Verify against the raw request body with a\n    5-minute timestamp tolerance.\n  docs: https://developers.justt.ai/docs/signature-verification\n\
  - name: mcp-oauth\n  type: oauth2\n  applies_to: the MCP endpoint at justt.ai/wp-json/mcp/mcp-oauth-server\n  authorization_server: https://justt.ai\n  authorization_endpoint: https://justt.ai/oauth/authorize\n  token_endpoint: https://justt.ai/oauth/token\n  revocation_endpoint: https://justt.ai/oauth/revoke\n  grant_types: [authorization_code, refresh_token]\n  pkce: S256\n  scopes: [mcp]\n  token_endpoint_auth_methods: [none]\n  sources:\n  - well-known/justt-oauth-authorization-server.json\n  - well-known/justt-oauth-protected-resource.json\n  note: >-\n    Discovered by probe, not documented. This OAuth surface belongs to the MCP\n    endpoint on the WordPress marketing host and has NOTHING to do with the\n    chargeback API, which never uses OAuth. Recorded so an agent does not attempt\n    an OAuth dance against api.justt.ai.\nauthorization_model:\n  scopes: false\n  roles: false\n  tenancy:\n    mechanism: reference-account-id request header\n    docs: https://developers.justt.ai/docs/reference-accounts\n\
  \    note: >-\n      One key can address multiple merchant accounts by setting the\n      reference-account-id header. There is no scope, permission or role system —\n      a key that can read chargebacks can also accept them, which is the\n      irreversible operation. Least-privilege is not expressible.\ntransport:\n  https_required: true\n  statement: >-\n    \"All our API calls must be transmitted over HTTPS. Calls made over plain HTTP\n    will not succeed.\"\ngaps:\n- The OpenAPI declares securitySchemes but leaves the top-level `security` array\n  empty and applies no security requirement to any operation, so a generated client\n  will not send credentials by default even though every call requires them.\n- No scopes, no per-key permissions, no key rotation or expiry policy is published.\n- No OpenID Connect discovery on any Justt host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/authentication/justt-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Company
- Payments
- Chargebacks
- Disputes
- Fraud
- Risk
- Financial Services
- E-Commerce
- Artificial Intelligence
- Webhooks
---
