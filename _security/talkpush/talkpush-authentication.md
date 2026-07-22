---
api_key_in:
- query
api_specs:
- filename: talkpush-openapi.json
  format: json
  label: Talkpush API
  slug: talkpush-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Talkpush Authentication
name_suffix: Authentication
oauth_flows: []
overview: TalkPush secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TalkPush
provider_slug: talkpush
scheme_count: 1
schemes:
- description: The API key provided for your application, passed as a query parameter on every API call. Contact TalkPush support to obtain or rotate a key.
  in: query
  name: ApiKeyQuery
  parameter: api_key
  required: true
  sources:
  - openapi/talkpush-openapi.json
  type: apiKey
slug: talkpush-authentication
source_filename: talkpush-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.talkpush.com/docs/getting-started\ndocs: https://docs.talkpush.com/docs/getting-started\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\n  notes: >-\n    The Talkpush API authenticates every request with an API key passed as the\n    query parameter `api_key`. The key is scoped to a company workspace; the base\n    URL is your company workspace subdomain, e.g.\n    https://{subdomain}.talkpush.com/api/talkpush_services. Keys are issued by\n    TalkPush support (cs@talkpush.com / admin@talkpush.com) and are not\n    self-service. No OAuth, OpenID Connect, or per-scope authorization surface is\n    documented; access is company-level via the single API key.\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  required: true\n  description: >-\n    The API key provided for your application, passed as a query parameter on\n    every API call. Contact TalkPush\
  \ support to obtain or rotate a key.\n  sources: [openapi/talkpush-openapi.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/authentication/talkpush-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Recruiting
- Recruitment Automation
- Human Resources
- Hiring
- Applicant Tracking
- Conversational AI
- Messaging
- CRM
---
