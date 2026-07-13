---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Goto Gojek Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoTo Group (Gojek + Tokopedia) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GoTo Group (Gojek + Tokopedia)
provider_slug: goto-gojek
scheme_count: 1
schemes:
- description: Server Key as username, empty password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/goto-gojek-openapi.yml
  type: http
slug: goto-gojek-authentication
source_filename: goto-gojek-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/goto-gojek-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Server Key as username, empty password\n  sources:\n  - openapi/goto-gojek-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goto-gojek/refs/heads/main/authentication/goto-gojek-authentication.yml
summary_line: http · 1 scheme
tags:
- Superapp
- Ride Hailing
- Food Delivery
- Last-Mile Logistics
- E-commerce
- Digital Payments
- Indonesia
- Southeast Asia
- Gojek
- Tokopedia
---
