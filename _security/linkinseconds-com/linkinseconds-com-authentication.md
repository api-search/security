---
anonymous_access: false
api_key_in: []
api_specs:
- filename: linkinseconds-com-analytics-api-openapi.yml
  format: yaml
  label: Link in Seconds Analytics API
  slug: linkinseconds-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkinseconds-com/openapi/linkinseconds-com-analytics-api-openapi.yml
- filename: linkinseconds-com-links-api-openapi.yml
  format: yaml
  label: Link in Seconds Links API
  slug: linkinseconds-com-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkinseconds-com/openapi/linkinseconds-com-links-api-openapi.yml
- filename: linkinseconds-com-status-api-openapi.yml
  format: yaml
  label: Link in Seconds Status API
  slug: linkinseconds-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkinseconds-com/openapi/linkinseconds-com-status-api-openapi.yml
- filename: linkinseconds-com-uploads-api-openapi.yml
  format: yaml
  label: Link in Seconds Uploads API
  slug: linkinseconds-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkinseconds-com/openapi/linkinseconds-com-uploads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Link in Seconds Authentication
name_suffix: Authentication
oauth_flows: []
overview: Link in Seconds secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Link in Seconds
provider_slug: linkinseconds-com
scheme_count: 1
schemes:
- description: API key from /dashboard/api-keys (starts with lis_).
  name: apiKey
  scheme: bearer
  sources:
  - openapi/linkinseconds-com-openapi.json
  type: http
slug: linkinseconds-com-authentication
source_filename: linkinseconds-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/linkinseconds-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: API key from /dashboard/api-keys (starts with lis_).\n  sources:\n  - openapi/linkinseconds-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/linkinseconds-com/authentication/linkinseconds-com-authentication.yml
summary_line: http · 1 scheme
tags:
- File Sharing
- Link Management
- Software-as-a-Service
- Cloud Storage
- Productivity
---
