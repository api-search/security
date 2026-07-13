---
api_key_in: []
api_specs:
- filename: sanity-openapi.yml
  format: yaml
  label: Sanity Query API
  slug: sanity-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanity/refs/heads/main/openapi/sanity-openapi.yml
- filename: sanity-webhooks-asyncapi.yml
  format: yaml
  label: Sanity Webhooks API
  slug: sanity-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanity/refs/heads/main/asyncapi/sanity-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sanity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sanity secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sanity
provider_slug: sanity
scheme_count: 1
schemes:
- description: Sanity project API token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sanity-openapi.yml
  type: http
slug: sanity-authentication
source_filename: sanity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sanity-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Sanity project API token\n  sources:\n  - openapi/sanity-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanity/refs/heads/main/authentication/sanity-authentication.yml
summary_line: http · 1 scheme
tags:
- Headless CMS
- Content Management
- GROQ
- Real-Time
- Structured Content
- Developer Platform
---
