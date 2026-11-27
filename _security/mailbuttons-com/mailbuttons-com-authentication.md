---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailbuttons-com-auth-api-openapi.yml
  format: yaml
  label: Mailbuttons Auth API
  slug: mailbuttons-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-auth-api-openapi.yml
- filename: mailbuttons-com-jmap-api-openapi.yml
  format: yaml
  label: Mailbuttons Jmap API
  slug: mailbuttons-com-jmap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-jmap-api-openapi.yml
- filename: mailbuttons-com-mailboxes-api-openapi.yml
  format: yaml
  label: Mailbuttons Mailboxes API
  slug: mailbuttons-com-mailboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-mailboxes-api-openapi.yml
- filename: mailbuttons-com-memory-api-openapi.yml
  format: yaml
  label: Mailbuttons Memory API
  slug: mailbuttons-com-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-memory-api-openapi.yml
- filename: mailbuttons-com-policy-api-openapi.yml
  format: yaml
  label: Mailbuttons Policy API
  slug: mailbuttons-com-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-policy-api-openapi.yml
- filename: mailbuttons-com-send-api-openapi.yml
  format: yaml
  label: Mailbuttons Send API
  slug: mailbuttons-com-send-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-send-api-openapi.yml
- filename: mailbuttons-com-threads-api-openapi.yml
  format: yaml
  label: Mailbuttons Threads API
  slug: mailbuttons-com-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-threads-api-openapi.yml
- filename: mailbuttons-com-webhooks-api-openapi.yml
  format: yaml
  label: Mailbuttons Webhooks API
  slug: mailbuttons-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Mailbuttons Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailbuttons secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mailbuttons
provider_slug: mailbuttons-com
scheme_count: 1
schemes:
- bearerFormat: API key
  name: apiKey
  scheme: bearer
  sources:
  - openapi/mailbuttons-com-openapi.json
  type: http
slug: mailbuttons-com-authentication
source_filename: mailbuttons-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/mailbuttons-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  sources:\n  - openapi/mailbuttons-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mailbuttons-com/authentication/mailbuttons-com-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- Quoting
---
