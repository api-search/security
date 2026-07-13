---
api_key_in: []
api_specs:
- filename: segment-public-api-openapi.yml
  format: yaml
  label: Segment Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-public-api-openapi.yml
- filename: segment-http-tracking-api-openapi.yml
  format: yaml
  label: Segment HTTP Tracking API
  slug: http-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-http-tracking-api-openapi.yml
- filename: segment-profile-api-openapi.yml
  format: yaml
  label: Segment Profile API
  slug: profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-profile-api-openapi.yml
- filename: segment-config-api-openapi.yml
  format: yaml
  label: Segment Config API
  slug: config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-config-api-openapi.yml
- filename: segment-pixel-tracking-api-openapi.yml
  format: yaml
  label: Segment Pixel Tracking API
  slug: pixel-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-pixel-tracking-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Segment Authentication
name_suffix: Authentication
oauth_flows: []
overview: segment secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: segment
provider_slug: segment
scheme_count: 2
schemes:
- description: Segment Config API access token. Note that as of early 2024, Segment has stopped issuing new Config API tokens.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/segment-config-api-openapi.yml
  - openapi/segment-public-api-openapi.yml
  type: http
- description: HTTP Basic authentication using the source write key as the username and an empty password. The write key is found in the Segment source settings.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/segment-http-tracking-api-openapi.yml
  - openapi/segment-profile-api-openapi.yml
  type: http
slug: segment-authentication
source_filename: segment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/segment-config-api-openapi.yml, openapi/segment-http-tracking-api-openapi.yml,\n  openapi/segment-profile-api-openapi.yml, openapi/segment-public-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Segment Config API access token. Note that as of early 2024, Segment has stopped\n    issuing new Config API tokens.\n  sources:\n  - openapi/segment-config-api-openapi.yml\n  - openapi/segment-public-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using the source write key as the username and an empty\n    password. The write key is found in the Segment source settings.\n  sources:\n  - openapi/segment-http-tracking-api-openapi.yml\n  - openapi/segment-profile-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/authentication/segment-authentication.yml
summary_line: http · 2 schemes
tags: []
---
