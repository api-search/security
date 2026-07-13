---
api_key_in: []
api_specs:
- filename: wistia-openapi.yml
  format: yaml
  label: Wistia Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-openapi.yml
- filename: wistia-asyncapi.yml
  format: yaml
  label: Wistia Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/asyncapi/wistia-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wistia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wistia secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wistia
provider_slug: wistia
scheme_count: 2
schemes:
- description: API access token sent as a Bearer token in the Authorization header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wistia-openapi.yml
  type: http
- description: HTTP Basic authentication using the API token as the password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/wistia-openapi.yml
  type: http
slug: wistia-authentication
source_filename: wistia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wistia-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API access token sent as a Bearer token in the Authorization header\n  sources:\n  - openapi/wistia-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using the API token as the password\n  sources:\n  - openapi/wistia-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/authentication/wistia-authentication.yml
summary_line: http · 2 schemes
tags:
- Video Hosting
- Video Marketing
- Video Analytics
- Lead Generation
- Webinars
- B2B Marketing
---
