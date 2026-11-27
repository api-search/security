---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: blotato-accounts-api-openapi.yml
  format: yaml
  label: Blotato Accounts API
  slug: blotato-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blotato/openapi/blotato-accounts-api-openapi.yml
- filename: blotato-analytics-api-openapi.yml
  format: yaml
  label: Blotato Analytics API
  slug: blotato-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blotato/openapi/blotato-analytics-api-openapi.yml
- filename: blotato-automations-api-openapi.yml
  format: yaml
  label: Blotato Automations API
  slug: blotato-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blotato/openapi/blotato-automations-api-openapi.yml
- filename: blotato-billing-api-openapi.yml
  format: yaml
  label: Blotato Billing API
  slug: blotato-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blotato/openapi/blotato-billing-api-openapi.yml
- filename: blotato-comments-api-openapi.yml
  format: yaml
  label: Blotato Comments API
  slug: blotato-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blotato/openapi/blotato-comments-api-openapi.yml
- filename: blotato-messaging-api-openapi.yml
  format: yaml
  label: Blotato Messaging API
  slug: blotato-messaging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blotato/openapi/blotato-messaging-api-openapi.yml
- filename: blotato-publishing-api-openapi.yml
  format: yaml
  label: Blotato Publishing API
  slug: blotato-publishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blotato/openapi/blotato-publishing-api-openapi.yml
- filename: blotato-video-api-openapi.yml
  format: yaml
  label: Blotato Video API
  slug: blotato-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blotato/openapi/blotato-video-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Blotato Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blotato secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blotato
provider_slug: blotato
scheme_count: 1
schemes:
- description: API key generated in Blotato Settings > API. Sent in the blotato-api-key header on every request. Keys may include trailing '=' padding that must be preserved.
  in: header
  name: blotatoApiKey
  parameter: blotato-api-key
  sources:
  - openapi/blotato-openapi.yml
  type: apiKey
slug: blotato-authentication
source_filename: blotato-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blotato-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: blotatoApiKey\n  type: apiKey\n  in: header\n  parameter: blotato-api-key\n  description: API key generated in Blotato Settings > API. Sent in the blotato-api-key header\n    on every request. Keys may include trailing '=' padding that must be preserved.\n  sources:\n  - openapi/blotato-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/blotato/authentication/blotato-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Social Media
- Publishing
- AI Content
- Automation
- Content Creation
---
