---
api_key_in: []
api_specs:
- filename: june-companies-api-openapi.yml
  format: yaml
  label: June Companies API
  slug: june-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/june/refs/heads/main/openapi/june-companies-api-openapi.yml
- filename: june-events-api-openapi.yml
  format: yaml
  label: June Events API
  slug: june-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/june/refs/heads/main/openapi/june-events-api-openapi.yml
- filename: june-page-views-api-openapi.yml
  format: yaml
  label: June Page Views API
  slug: june-page-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/june/refs/heads/main/openapi/june-page-views-api-openapi.yml
- filename: june-users-api-openapi.yml
  format: yaml
  label: June Users API
  slug: june-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/june/refs/heads/main/openapi/june-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: June Authentication
name_suffix: Authentication
oauth_flows: []
overview: June secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: June
provider_slug: june
scheme_count: 1
schemes:
- description: Provide your workspace write key as the username via HTTP Basic Auth. Obtain the write key from your June workspace settings.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/june-tracking-api-openapi.yml
  type: http
slug: june-authentication
source_filename: june-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/june-tracking-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Provide your workspace write key as the username via HTTP Basic Auth. Obtain\n    the write key from your June workspace settings.\n  sources:\n  - openapi/june-tracking-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/june/refs/heads/main/authentication/june-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Product Analytics
- B2B SaaS
- Event Tracking
- Segment Compatible
- Retention
- Feature Adoption
- Activation
---
