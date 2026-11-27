---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CaptureOneAI Authentication
name_suffix: Authentication
oauth_flows: []
overview: CaptureOneAI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CaptureOneAI
provider_slug: captureoneai-com
scheme_count: 2
schemes:
- description: 'X-API-Key Header (recommended) X-API-Key: REDACTED_STRIPE_KEY'
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  recommended: true
  type: apiKey
- description: 'Authorization Bearer token Authorization: Bearer REDACTED_STRIPE_KEY'
  name: BearerToken
  scheme: bearer
  type: http
slug: captureoneai-com-authentication
source_filename: captureoneai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: CaptureOneAI authentication\ngenerated: '2026-11-03'\nmethod: searched\nsource: https://captureoneai.com/docs\ndocs: https://captureoneai.com/docs\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  recommended: true\n  description: 'X-API-Key Header (recommended) X-API-Key: REDACTED_STRIPE_KEY'\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: 'Authorization Bearer token Authorization: Bearer REDACTED_STRIPE_KEY'\nkey_prefixes:\n- sk_live_\nkey_management: Keys are generated or copied in the dashboard; \"Rotate it from your dashboard if it's compromised.\"\nmcp:\n  endpoint: https://captureoneai.com/mcp\n  scheme: bearer\n  note: Per https://captureoneai.com/integrations/mcp, initialize and tools/list answer without an API key; only tools/call needs a key.\n"
source_yaml_url: https://artifacts.apis.io/captureoneai-com/authentication/captureoneai-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Website Monitoring
- Change Detection
- Screenshots
- PDF Generation
- Web Capture
- Artificial Intelligence
- Alerts
---
