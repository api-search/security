---
api_key_in:
- header
api_specs:
- filename: teambridge-openapi-original.json
  format: json
  label: Teambridge External API
  slug: teambridge-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teambridge/refs/heads/main/openapi/teambridge-openapi-original.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Teambridge Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Teambridge secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Teambridge
provider_slug: teambridge
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://teambridge.us.auth0.com/oauth/token
  name: OAuth2
  sources:
  - openapi/teambridge-openapi-original.json
  type: oauth2
- description: 'HMAC-SHA256 signature for webhook authentication. The signature is computed from

    the concatenation of the timestamp and request body: `{timestamp}.{body}`.

    The signature header value includes the scheme prefix: `sha256={hex_signature}`.


    Webhook consumers must verify this signature using their webhook secret to ensure

    the request originated from Teambridge.'
  in: header
  name: WebhookSignature
  parameter: X-Webhook-Signature
  sources:
  - openapi/teambridge-openapi-original.json
  type: apiKey
slug: teambridge-authentication
source_filename: teambridge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/teambridge-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://teambridge.us.auth0.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/teambridge-openapi-original.json\n- name: WebhookSignature\n  type: apiKey\n  in: header\n  parameter: X-Webhook-Signature\n  description: |-\n    HMAC-SHA256 signature for webhook authentication. The signature is computed from\n    the concatenation of the timestamp and request body: `{timestamp}.{body}`.\n    The signature header value includes the scheme prefix: `sha256={hex_signature}`.\n\n    Webhook consumers must verify this signature using their webhook secret to ensure\n    the request originated from Teambridge.\n  sources:\n  - openapi/teambridge-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teambridge/refs/heads/main/authentication/teambridge-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Workforce Management
- Scheduling
- Time Tracking
- Payroll
- HR
- Frontline
- Webhooks
---
