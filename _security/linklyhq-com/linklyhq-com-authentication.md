---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: linklyhq-com-clicks-api-openapi.yml
  format: yaml
  label: Linkly Clicks API
  slug: linklyhq-com-clicks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linklyhq-com/openapi/linklyhq-com-clicks-api-openapi.yml
- filename: linklyhq-com-conversions-api-openapi.yml
  format: yaml
  label: Linkly Conversions API
  slug: linklyhq-com-conversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linklyhq-com/openapi/linklyhq-com-conversions-api-openapi.yml
- filename: linklyhq-com-domains-api-openapi.yml
  format: yaml
  label: Linkly Domains API
  slug: linklyhq-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linklyhq-com/openapi/linklyhq-com-domains-api-openapi.yml
- filename: linklyhq-com-links-api-openapi.yml
  format: yaml
  label: Linkly Links API
  slug: linklyhq-com-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linklyhq-com/openapi/linklyhq-com-links-api-openapi.yml
- filename: linklyhq-com-webhooks-api-openapi.yml
  format: yaml
  label: Linkly Webhooks API
  slug: linklyhq-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linklyhq-com/openapi/linklyhq-com-webhooks-api-openapi.yml
- filename: linklyhq-com-workspaces-api-openapi.yml
  format: yaml
  label: Linkly Workspaces API
  slug: linklyhq-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linklyhq-com/openapi/linklyhq-com-workspaces-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Linkly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Linkly secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Linkly
provider_slug: linklyhq-com
scheme_count: 3
schemes:
- description: 'Authorization: Bearer <API key>. Find the key under Workspace settings > API in app.linklyhq.com.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/linklyhq-com-openapi.json
  type: http
- description: API key as the username, empty password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/linklyhq-com-openapi.json
  type: http
- description: Query-string fallback for quick tests only.
  in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/linklyhq-com-openapi.json
  type: apiKey
slug: linklyhq-com-authentication
source_filename: linklyhq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/linklyhq-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer <API key>. Find the key under Workspace settings > API\n    in app.linklyhq.com.'\n  sources:\n  - openapi/linklyhq-com-openapi.json\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: API key as the username, empty password.\n  sources:\n  - openapi/linklyhq-com-openapi.json\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Query-string fallback for quick tests only.\n  sources:\n  - openapi/linklyhq-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/linklyhq-com/authentication/linklyhq-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- URL Shorteners
- Link Tracking
- Analytics
- Branded Links
- QR Codes
- Company
---
