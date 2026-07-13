---
api_key_in: []
api_specs:
- filename: appcues-openapi.yml
  format: yaml
  label: Appcues Public API
  slug: appcues-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Appcues Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appcues secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Appcues
provider_slug: appcues
scheme_count: 1
schemes:
- description: HTTP Basic authentication using API_KEY as username and API_SECRET as password.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/appcues-openapi.yml
  type: http
slug: appcues-authentication
source_filename: appcues-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/appcues-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using API_KEY as username and API_SECRET as password.\n  sources:\n  - openapi/appcues-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/authentication/appcues-authentication.yml
summary_line: http · 1 scheme
tags:
- Product
- Onboarding
- In-App Guidance
- Analytics
- Customer Success
---
