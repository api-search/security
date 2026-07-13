---
api_key_in: []
api_specs:
- filename: courier-openapi.yml
  format: yaml
  label: Courier Send API
  slug: courier-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-openapi.yml
- filename: courier-openapi.yml
  format: yaml
  label: Courier User Profiles API
  slug: courier-user-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-openapi.yml
- filename: courier-openapi.yml
  format: yaml
  label: Courier Lists API
  slug: courier-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-openapi.yml
- filename: courier-openapi.yml
  format: yaml
  label: Courier Events API
  slug: courier-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-openapi.yml
- filename: courier-openapi.yml
  format: yaml
  label: Courier Brands API
  slug: courier-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-openapi.yml
- filename: courier-openapi.yml
  format: yaml
  label: Courier Authentication API
  slug: courier-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-openapi.yml
- filename: courier-asyncapi.yml
  format: yaml
  label: Courier Inbox Real-Time API
  slug: courier-inbox-real-time-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/asyncapi/courier-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Courier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Courier secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Courier
provider_slug: courier
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/courier-openapi.yml
  type: http
slug: courier-authentication
source_filename: courier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/courier-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/courier-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/authentication/courier-authentication.yml
summary_line: http · 1 scheme
tags:
- Notifications
- Email
- SMS
- Push
- API
---
