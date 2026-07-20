---
api_key_in: []
api_specs:
- filename: lanzatech-wordpress-openapi.yml
  format: yaml
  label: LanzaTech WordPress REST API
  slug: wordpress
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lanzatech/refs/heads/main/openapi/lanzatech-wordpress-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lanzatech Authentication
name_suffix: Authentication
oauth_flows: []
overview: LanzaTech secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LanzaTech
provider_slug: lanzatech
scheme_count: 1
schemes:
- description: WordPress application passwords, advertised by the API root document at https://lanzatech.com/wp-json/ (authentication.application-passwords.endpoints.authorization = https://lanzatech.com/wp-admin/authorize-application.php). Sent as HTTP Basic credentials. Only required for write operations; all read operations captured here are public.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/lanzatech-wordpress-openapi.yml
  type: http
slug: lanzatech-authentication
source_filename: lanzatech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lanzatech-wordpress-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application passwords, advertised by the API root document at https://lanzatech.com/wp-json/\n    (authentication.application-passwords.endpoints.authorization = https://lanzatech.com/wp-admin/authorize-application.php).\n    Sent as HTTP Basic credentials. Only required for write operations; all read operations\n    captured here are public.\n  sources:\n  - openapi/lanzatech-wordpress-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lanzatech/refs/heads/main/authentication/lanzatech-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Carbon Capture
- Climate Tech
- Sustainability
- Synthetic Biology
- Energy
- Chemicals
- Sustainable Aviation Fuel
- Manufacturing
- Content
---
