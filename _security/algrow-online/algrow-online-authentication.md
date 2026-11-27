---
anonymous_access: false
api_key_in: []
api_specs:
- filename: algrow-online-openapi-generated.yml
  format: yaml
  label: Algrow API
  slug: algrow-online-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algrow-online/openapi/_ae-authored/algrow-online-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Algrow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Algrow declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Algrow
provider_slug: algrow-online
scheme_count: 3
schemes:
- description: Bearer algrow_...
  in: header
  name: Authorization
  type: apiKey
- description: API key as query parameter
  in: query
  name: api_key
  type: apiKey
- description: API key in multipart form body
  in: formData
  name: api_key
  type: apiKey
slug: algrow-online-authentication
source_filename: algrow-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://algrow.online/docs/api-keys.md\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer algrow_...\"\n  - type: apiKey\n    name: api_key\n    in: query\n    description: \"API key as query parameter\"\n  - type: apiKey\n    name: api_key\n    in: formData\n    description: \"API key in multipart form body\"\n"
source_yaml_url: https://artifacts.apis.io/algrow-online/authentication/algrow-online-authentication.yml
summary_line: 3 schemes
tags:
- YouTube
- Content Creation
- Artificial Intelligence
- Analytics
- Marketing
---
