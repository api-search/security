---
api_key_in: []
api_specs:
- filename: vibes-platform-openapi.yml
  format: yaml
  label: Vibes Platform API
  slug: vibes-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-openapi.yml
- filename: vibes-connect-openapi.yml
  format: yaml
  label: Vibes Connect API
  slug: vibes-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-connect-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vibes Platform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vibes Platform secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vibes Platform
provider_slug: vibes-platform
scheme_count: 1
schemes:
- description: HTTP Basic Authentication. Combine the username and password into a "username:password" string, encode it using Base64, and add the Authorization HTTP header set to "Basic " plus the encoded string.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/vibes-connect-openapi.yml
  - openapi/vibes-platform-openapi.yml
  type: http
slug: vibes-platform-authentication
source_filename: vibes-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vibes-connect-openapi.yml, openapi/vibes-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication. Combine the username and password into a \"username:password\"\n    string, encode it using Base64, and add the Authorization HTTP header set to \"Basic \" plus\n    the encoded string.\n  sources:\n  - openapi/vibes-connect-openapi.yml\n  - openapi/vibes-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/authentication/vibes-platform-authentication.yml
summary_line: http · 1 scheme
tags:
- Mobile Marketing
- Mobile Messaging
- Push Notifications
- SMS
- MMS
- Broadcast Messaging
- Acquisition Campaigns
- Subscription Management
- Wallet Passes
- RCS
---
