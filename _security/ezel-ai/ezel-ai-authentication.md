---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ezel-ai-openapi-generated.yml
  format: yaml
  label: Ezel API
  slug: ezel-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ezel-ai/openapi/_ae-authored/ezel-ai-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ezel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ezel declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ezel
provider_slug: ezel-ai
scheme_count: 2
schemes:
- description: Personal API key sent as a Bearer token in the Authorization header.
  name: Authorization
  scheme: bearer
  type: http
- description: Alternative header for tools that cannot set Authorization.
  in: header
  name: X-API-Key
  type: apiKey
slug: ezel-ai-authentication
source_filename: ezel-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://ezel.ai/docs#authentication\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Personal API key sent as a Bearer token in the Authorization header.\"\n    name: Authorization\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    description: \"Alternative header for tools that cannot set Authorization.\"\n"
source_yaml_url: https://artifacts.apis.io/ezel-ai/authentication/ezel-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Legal Tech
- Software-as-a-Service
- Platform
- Company
---
