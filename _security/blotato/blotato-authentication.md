---
api_key_in:
- header
api_specs:
- filename: blotato-openapi.yml
  format: yaml
  label: Blotato Media Upload API
  slug: blotato-media-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/openapi/blotato-openapi.yml
- filename: blotato-openapi.yml
  format: yaml
  label: Blotato Posts Publishing API
  slug: blotato-posts-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/openapi/blotato-openapi.yml
- filename: blotato-openapi.yml
  format: yaml
  label: Blotato AI Content API
  slug: blotato-ai-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/openapi/blotato-openapi.yml
- filename: blotato-openapi.yml
  format: yaml
  label: Blotato Accounts API
  slug: blotato-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/openapi/blotato-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/authentication/blotato-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Social Media
- Publishing
- AI Content
- Automation
- Content Creation
---
