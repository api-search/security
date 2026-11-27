---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: lots-blog-lots-blog-api-openapi.yml
  format: yaml
  label: LotsBlog Lots.Blog API
  slug: lots-blog-lots-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lots-blog/openapi/lots-blog-lots-blog-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: LotsBlog Authentication
name_suffix: Authentication
oauth_flows: []
overview: LotsBlog secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LotsBlog
provider_slug: lots-blog
scheme_count: 1
schemes:
- description: 'API key for authentication. Format: REDACTED_STRIPE_KEY'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/lots-blog-openapi.json
  type: apiKey
slug: lots-blog-authentication
source_filename: lots-blog-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/lots-blog-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'API key for authentication. Format: REDACTED_STRIPE_KEY'\n  sources:\n  - openapi/lots-blog-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lots-blog/authentication/lots-blog-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Blogging
- Content Creation
- Automation
---
