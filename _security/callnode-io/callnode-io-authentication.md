---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: callnode-io-call-records-api-openapi.yml
  format: yaml
  label: CallNode Call Records API
  slug: callnode-io-call-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-call-records-api-openapi.yml
- filename: callnode-io-email-api-openapi.yml
  format: yaml
  label: CallNode Email API
  slug: callnode-io-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-email-api-openapi.yml
- filename: callnode-io-faxes-api-openapi.yml
  format: yaml
  label: CallNode Faxes API
  slug: callnode-io-faxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-faxes-api-openapi.yml
- filename: callnode-io-messaging-api-openapi.yml
  format: yaml
  label: CallNode Messaging API
  slug: callnode-io-messaging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-messaging-api-openapi.yml
- filename: callnode-io-outbound-calls-api-openapi.yml
  format: yaml
  label: CallNode Outbound Calls API
  slug: callnode-io-outbound-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-outbound-calls-api-openapi.yml
- filename: callnode-io-phone-numbers-api-openapi.yml
  format: yaml
  label: CallNode Phone Numbers API
  slug: callnode-io-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-phone-numbers-api-openapi.yml
- filename: callnode-io-sip-trunks-api-openapi.yml
  format: yaml
  label: CallNode SIP Trunks API
  slug: callnode-io-sip-trunks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-sip-trunks-api-openapi.yml
- filename: callnode-io-wholesale-api-openapi.yml
  format: yaml
  label: CallNode Wholesale API
  slug: callnode-io-wholesale-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callnode-io/openapi/callnode-io-wholesale-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CallNode Authentication
name_suffix: Authentication
oauth_flows: []
overview: CallNode secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CallNode
provider_slug: callnode-io
scheme_count: 3
schemes:
- description: Your API key, e.g. `cn_live_...`.
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/callnode-io-openapi.yml
  type: apiKey
- description: Unix seconds as a string, used as the signature prefix.
  in: header
  name: TimestampAuth
  parameter: X-Timestamp
  sources:
  - openapi/callnode-io-openapi.yml
  type: apiKey
- description: '`hex(HMAC_SHA256(apiSecret, timestamp + "\n" + rawBody))`.'
  in: header
  name: SignatureAuth
  parameter: X-Signature
  sources:
  - openapi/callnode-io-openapi.yml
  type: apiKey
slug: callnode-io-authentication
source_filename: callnode-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://callnode.io/docs/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Your API key, e.g. `cn_live_...`.\n  sources:\n  - openapi/callnode-io-openapi.yml\n- name: TimestampAuth\n  type: apiKey\n  in: header\n  parameter: X-Timestamp\n  description: Unix seconds as a string, used as the signature prefix.\n  sources:\n  - openapi/callnode-io-openapi.yml\n- name: SignatureAuth\n  type: apiKey\n  in: header\n  parameter: X-Signature\n  description: '`hex(HMAC_SHA256(apiSecret, timestamp + \"\\n\" + rawBody))`.'\n  sources:\n  - openapi/callnode-io-openapi.yml\ndocs: https://callnode.io/docs/authentication\nsigning:\n  algorithm: HMAC-SHA256\n  string_to_sign: timestamp + \"\\n\" + body\n  header: X-Signature\n  encoding: hex\n  clock_skew: Must be within ±300s of server clock.\n  skew_error: 401 clock_skew\n\
  \  skew_header: X-Server-Time\nkey_prefixes:\n- prefix: cn_live_\n  environment: live\n- prefix: cn_test_\n  environment: test\nsecret_rotation: When you rotate a key's secret from the dashboard, the previous secret remains valid for 24 hours .\nnotes:\n- The secret is shown exactly once at creation/rotation.\n- Errors page names a key scope, e.g. outbound:call (403 scope_denied); no scope reference page is published for the REST API.\n- The MCP server (https://mcp.callnode.io/mcp) separately supports OAuth sign-in or a Bearer token per the MCP docs.\n"
source_yaml_url: https://artifacts.apis.io/callnode-io/authentication/callnode-io-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Voice AI
- Telephony
- Phone Numbers
- SMS
- Webhook
- SIP Trunking
- AI Agents
- Communications
---
