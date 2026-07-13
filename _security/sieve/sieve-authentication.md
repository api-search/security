---
api_key_in:
- header
api_specs:
- filename: sieve-openapi.yml
  format: yaml
  label: Sieve Jobs Push API
  slug: sieve-jobs-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/openapi/sieve-openapi.yml
- filename: sieve-openapi.yml
  format: yaml
  label: Sieve Jobs Status API
  slug: sieve-jobs-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/openapi/sieve-openapi.yml
- filename: sieve-openapi.yml
  format: yaml
  label: Sieve Functions API
  slug: sieve-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/openapi/sieve-openapi.yml
- filename: sieve-openapi.yml
  format: yaml
  label: Sieve Webhooks API
  slug: sieve-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/openapi/sieve-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sieve Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sieve secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sieve
provider_slug: sieve
scheme_count: 1
schemes:
- description: The Sieve API key to authenticate with.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/sieve-openapi.yml
  type: apiKey
slug: sieve-authentication
source_filename: sieve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sieve-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: The Sieve API key to authenticate with.\n  sources:\n  - openapi/sieve-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/authentication/sieve-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Video
- Audio
- Media Processing
- Async Jobs
---
