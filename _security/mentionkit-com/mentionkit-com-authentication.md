---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mentionkit-com-keywords-api-openapi.yml
  format: yaml
  label: Mentionkit Keywords API
  slug: mentionkit-com-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentionkit-com/openapi/mentionkit-com-keywords-api-openapi.yml
- filename: mentionkit-com-mentions-api-openapi.yml
  format: yaml
  label: Mentionkit Mentions API
  slug: mentionkit-com-mentions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentionkit-com/openapi/mentionkit-com-mentions-api-openapi.yml
- filename: mentionkit-com-organization-api-openapi.yml
  format: yaml
  label: Mentionkit Organization API
  slug: mentionkit-com-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentionkit-com/openapi/mentionkit-com-organization-api-openapi.yml
- filename: mentionkit-com-projects-api-openapi.yml
  format: yaml
  label: Mentionkit Projects API
  slug: mentionkit-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentionkit-com/openapi/mentionkit-com-projects-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Mentionkit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mentionkit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mentionkit
provider_slug: mentionkit-com
scheme_count: 1
schemes:
- bearerFormat: APIKey
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mentionkit-com-openapi.json
  type: http
slug: mentionkit-com-authentication
source_filename: mentionkit-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mentionkit-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: APIKey\n  sources:\n  - openapi/mentionkit-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mentionkit-com/authentication/mentionkit-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Social Listening
- Brand Monitoring
- Webhook
- Software-as-a-Service
---
