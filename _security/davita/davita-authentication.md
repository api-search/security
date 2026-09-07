---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: davita-wp-rest.yml
  format: yaml
  label: DaVita Web REST API
  slug: davita-web-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/davita/refs/heads/main/openapi/davita-wp-rest.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Davita Authentication
name_suffix: Authentication
oauth_flows: []
overview: DaVita secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DaVita
provider_slug: davita
scheme_count: 2
schemes:
- description: 'WordPress Application Passwords. Authorization endpoint declared by the index: https://davita.com/wp-admin/authorize-application.php. Not offered to the public; write routes are staff-only.'
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/davita-wp-rest.yml
  type: http
- description: WordPress cookie authentication nonce, accepted per the Access-Control-Allow-Headers response header. Browser/session only.
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/davita-wp-rest.yml
  type: apiKey
slug: davita-authentication
source_filename: davita-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/davita-wp-rest.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: 'WordPress Application Passwords. Authorization endpoint declared by the index:\n    https://davita.com/wp-admin/authorize-application.php. Not offered to the public; write\n    routes are staff-only.'\n  sources:\n  - openapi/davita-wp-rest.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress cookie authentication nonce, accepted per the Access-Control-Allow-Headers\n    response header. Browser/session only.\n  sources:\n  - openapi/davita-wp-rest.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/davita/refs/heads/main/authentication/davita-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Chronic Kidney Disease
- Dialysis
- Fortune 500
- Healthcare
- Home Dialysis
- Hospital Partnerships
- Integrated Kidney Care
- Kidney Care
- Nutrition
- Patient Education
- Recipes
---
