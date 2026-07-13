---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: GOV.UK Notify Notifications API
  slug: notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gov-uk-notify/refs/heads/main/openapi/openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gov Uk Notify Authentication
name_suffix: Authentication
oauth_flows: []
overview: GOV.UK Notify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GOV.UK Notify
provider_slug: gov-uk-notify
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token signed with HS256 using the service API key secret. Tokens are short-lived and must include iss (service ID), iat (issued at), and exp (expiry) claims.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: gov-uk-notify-authentication
source_filename: gov-uk-notify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token signed with HS256 using the service API key secret. Tokens are short-lived\n    and must include iss (service ID), iat (issued at), and exp (expiry) claims.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gov-uk-notify/refs/heads/main/authentication/gov-uk-notify-authentication.yml
summary_line: http · 1 scheme
tags:
- Notifications
- Email
- SMS
- Text Messages
- Letters
- Government
- United Kingdom
- Public Sector
- GDS
- REST
---
