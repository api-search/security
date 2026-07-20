---
api_key_in: []
api_specs:
- filename: crescendo-lab-maacgo-openapi.yaml
  format: yaml
  label: MAAC Go API
  slug: maac-go-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crescendo-lab/refs/heads/main/openapi/crescendo-lab-maacgo-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Crescendo Lab Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crescendo Lab secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crescendo Lab
provider_slug: crescendo-lab
scheme_count: 1
schemes:
- description: '`Authorization: Bearer <api_key>`. Production keys start with `sk_live_`,

    test keys with `sk_test_` for environment separation. Sending still follows

    the account wallet and deployment adapter settings.'
  format: Bearer <api_key>
  header: Authorization
  key_prefixes:
  - sk_live_
  - sk_test_
  name: bearerAuth
  obtain: Generated on signup; managed in the dashboard at https://sms.cresclab.com/app.html#transactional
  scheme: bearer
  scope_note: API keys are scoped (e.g. sms.read) and wallet-backed; a read-only key cannot call send endpoints. Scopes gate which MCP tools succeed.
  scoped: true
  sources:
  - openapi/crescendo-lab-maacgo-openapi.yaml
  - https://sms.cresclab.com/developers.html
  type: http
slug: crescendo-lab-authentication
source_filename: crescendo-lab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/crescendo-lab-maacgo-openapi.yaml\ndocs: https://sms.cresclab.com/developers.html\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Bearer <api_key>'\n  key_prefixes:\n  - sk_live_\n  - sk_test_\n  obtain: Generated on signup; managed in the dashboard at https://sms.cresclab.com/app.html#transactional\n  scoped: true\n  scope_note: >-\n    API keys are scoped (e.g. sms.read) and wallet-backed; a read-only key\n    cannot call send endpoints. Scopes gate which MCP tools succeed.\n  description: |-\n    `Authorization: Bearer <api_key>`. Production keys start with `sk_live_`,\n    test keys with `sk_test_` for environment separation. Sending still follows\n    the account wallet and deployment adapter settings.\n  sources:\n  - openapi/crescendo-lab-maacgo-openapi.yaml\n  - https://sms.cresclab.com/developers.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crescendo-lab/refs/heads/main/authentication/crescendo-lab-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- SMS
- Messaging
- Marketing Automation
- Customer Engagement
- Taiwan
- Omnichannel
- MCP
---
