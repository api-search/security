---
api_key_in:
- query
api_specs:
- filename: talkpush-agents-api-api-openapi.yml
  format: yaml
  label: TalkPush Agents API API
  slug: talkpush-agents-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-agents-api-api-openapi.yml
- filename: talkpush-calls-api-api-openapi.yml
  format: yaml
  label: TalkPush Calls API API
  slug: talkpush-calls-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-calls-api-api-openapi.yml
- filename: talkpush-campaigns-api-api-openapi.yml
  format: yaml
  label: TalkPush Campaigns API API
  slug: talkpush-campaigns-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-campaigns-api-api-openapi.yml
- filename: talkpush-candidate-attributes-api-api-openapi.yml
  format: yaml
  label: TalkPush Candidate Attributes API API
  slug: talkpush-candidate-attributes-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-candidate-attributes-api-api-openapi.yml
- filename: talkpush-document-tags-api-api-openapi.yml
  format: yaml
  label: TalkPush Document Tags API API
  slug: talkpush-document-tags-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-document-tags-api-api-openapi.yml
- filename: talkpush-folders-api-api-openapi.yml
  format: yaml
  label: TalkPush Folders API API
  slug: talkpush-folders-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-folders-api-api-openapi.yml
- filename: talkpush-labels-api-api-openapi.yml
  format: yaml
  label: TalkPush Labels API API
  slug: talkpush-labels-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-labels-api-api-openapi.yml
- filename: talkpush-leads-api-api-openapi.yml
  format: yaml
  label: TalkPush Leads API API
  slug: talkpush-leads-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-leads-api-api-openapi.yml
- filename: talkpush-managers-api-api-openapi.yml
  format: yaml
  label: TalkPush Managers API API
  slug: talkpush-managers-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-managers-api-api-openapi.yml
- filename: talkpush-message-templates-api-api-openapi.yml
  format: yaml
  label: TalkPush Message Templates API API
  slug: talkpush-message-templates-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-message-templates-api-api-openapi.yml
- filename: talkpush-messaging-api-api-openapi.yml
  format: yaml
  label: TalkPush Messaging API API
  slug: talkpush-messaging-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-messaging-api-api-openapi.yml
- filename: talkpush-movement-reasons-api-api-openapi.yml
  format: yaml
  label: TalkPush Movement Reasons API API
  slug: talkpush-movement-reasons-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-movement-reasons-api-api-openapi.yml
- filename: talkpush-requisition-management-system-api-openapi.yml
  format: yaml
  label: TalkPush Requisition Management System API
  slug: talkpush-requisition-management-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-requisition-management-system-api-openapi.yml
- filename: talkpush-tokens-api-api-openapi.yml
  format: yaml
  label: TalkPush Tokens API API
  slug: talkpush-tokens-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkpush/refs/heads/main/openapi/talkpush-tokens-api-api-openapi.yml
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
