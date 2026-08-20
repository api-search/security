---
api_key_in: []
api_specs:
- filename: lorikeet-conversations-api-openapi.yml
  format: yaml
  label: Lorikeet Conversations API
  slug: lorikeet-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-conversations-api-openapi.yml
- filename: lorikeet-knowledge-api-openapi.yml
  format: yaml
  label: Lorikeet Knowledge API
  slug: lorikeet-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-knowledge-api-openapi.yml
- filename: lorikeet-messages-api-openapi.yml
  format: yaml
  label: Lorikeet Messages API
  slug: lorikeet-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-messages-api-openapi.yml
- filename: lorikeet-webhooks-api-openapi.yml
  format: yaml
  label: Lorikeet Webhooks API
  slug: lorikeet-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lorikeet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lorikeet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lorikeet
provider_slug: lorikeet
scheme_count: 1
schemes:
- description: 'Bearer API key issued to your Lorikeet account. Send as `Authorization: Bearer <API_KEY>`. Lorikeet also supports OAuth2, JWT bearer, Basic, HMAC, and M2M flows for tool/action integrations into your systems; those secure Lorikeet''s outbound calls rather than this inbound management API.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lorikeet-openapi.yml
  type: http
slug: lorikeet-authentication
source_filename: lorikeet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lorikeet-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer API key issued to your Lorikeet account. Send as `Authorization: Bearer\n    <API_KEY>`. Lorikeet also supports OAuth2, JWT bearer, Basic, HMAC, and M2M flows for tool/action\n    integrations into your systems; those secure Lorikeet''s outbound calls rather than this\n    inbound management API.'\n  sources:\n  - openapi/lorikeet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/authentication/lorikeet-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Customer-Support
- AI Agent
- Support Automation
- Workflows
- Help Desk
---
