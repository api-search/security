---
api_key_in: []
api_specs:
- filename: api_v2.json
  format: json
  label: Instantly Campaigns API
  slug: campaigns-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Leads API
  slug: leads-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Accounts API
  slug: accounts-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Email Verification API
  slug: email-verification-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Inbox Placement Test API
  slug: inbox-placement-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Analytics API
  slug: analytics-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly API Keys API
  slug: api-keys-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Workspaces API
  slug: workspaces-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Instantly Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Instantly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Instantly
provider_slug: instantly-ai
scheme_count: 1
schemes:
- bearerFormat: API key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/instantly-ai-openapi.yml
  type: http
slug: instantly-ai-authentication
source_filename: instantly-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/instantly-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  sources:\n  - openapi/instantly-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instantly-ai/refs/heads/main/authentication/instantly-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Cold Email
- Outbound
- Sales
- Deliverability
- Lead Database
- Email Verification
- Webhooks
---
