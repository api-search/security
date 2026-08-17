---
api_key_in:
- header
api_specs:
- filename: wideo-automation-api-openapi.yml
  format: yaml
  label: Wideo Automation API
  slug: wideo-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wideo/refs/heads/main/openapi/wideo-automation-api-openapi.yml
- filename: wideo-batch-api-openapi.yml
  format: yaml
  label: Wideo Batch API
  slug: wideo-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wideo/refs/heads/main/openapi/wideo-batch-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Wideo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wideo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wideo
provider_slug: wideo
scheme_count: 1
schemes:
- description: API key in UUID form, scoped to a specific account and permission set. Generated assets are isolated by account and stored securely.
  docs: https://wideo.co/api-documentation/
  example_shape: 12345678-1234-1234-1234-123456789012
  format: UUID
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - https://wideo.co/api-documentation/
  - openapi/wideo-automation-api-openapi.yml
  - openapi/wideo-batch-api-openapi.yml
  type: apiKey
slug: wideo-authentication
source_filename: wideo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://wideo.co/api-documentation/\ndocs: https://wideo.co/api-documentation/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  format: UUID\n  description: >-\n    API key in UUID form, scoped to a specific account and permission set.\n    Generated assets are isolated by account and stored securely.\n  example_shape: '12345678-1234-1234-1234-123456789012'\n  docs: https://wideo.co/api-documentation/\n  sources:\n  - https://wideo.co/api-documentation/\n  - openapi/wideo-automation-api-openapi.yml\n  - openapi/wideo-batch-api-openapi.yml\nissuance:\n  self_serve: false\n  path: '\"Request API access\" form on https://wideo.co/api-documentation/'\n  note: >-\n    No key can be obtained without a sales conversation. Every tier, including the\n    published paid tiers, is entered through the request form; there is no\n    dashboard-issued\
  \ key documented.\nrotation:\n  documented: false\n  note: No key rotation, expiry, or revocation procedure is published.\nobserved:\n  unauthenticated_response:\n    status: 403\n    body: '{\"message\":\"Missing Authentication Token\"}'\n    header: 'x-amzn-errortype: MissingAuthenticationTokenException'\n    url: https://automationapi.wideo.co/batch\n    probed: '2026-08-13'\ngaps:\n- >-\n  The legacy /automation/* code samples published on https://wideo.co/api/ send\n  only a Content-Type header and no x-api-key, so the published documentation does\n  not consistently state that the legacy pair requires a key.\n- No OAuth, OIDC or scoped-permission surface exists; see conformance/wideo-conformance.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wideo/refs/heads/main/authentication/wideo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Video
- Video Automation
- Content Creation
- Media
- Marketing
- Templates
- No-Code
---
