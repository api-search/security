---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: boston-properties-wordpress-rest-openapi.yml
  format: yaml
  label: BXP WordPress REST API
  slug: bxp-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boston-properties/refs/heads/main/openapi/boston-properties-wordpress-rest-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Boston Properties Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boston Properties (BXP) secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Boston Properties (BXP)
provider_slug: boston-properties
scheme_count: 2
schemes:
- description: WordPress application passwords, advertised by the site's own discovery document at https://www.bxp.com/wp-json/ (authentication.application-passwords.endpoints.authorization = https://www.bxp.com/wp-admin/authorize-application.php). Issued only to WordPress user accounts on the BXP site; not available to third parties.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/boston-properties-wordpress-rest-openapi.yml
  type: http
- description: WordPress logged-in cookie plus an X-WP-Nonce header. Advertised by the Access-Control-Allow-Headers response header observed on https://www.bxp.com/wp-json/wp/v2/pages (2026-09-04).
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/boston-properties-wordpress-rest-openapi.yml
  type: apiKey
slug: boston-properties-authentication
source_filename: boston-properties-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: derived\nsource: openapi/boston-properties-wordpress-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: WordPress application passwords, advertised by the site's own discovery document\n    at https://www.bxp.com/wp-json/ (authentication.application-passwords.endpoints.authorization\n    = https://www.bxp.com/wp-admin/authorize-application.php). Issued only to WordPress user\n    accounts on the BXP site; not available to third parties.\n  sources:\n  - openapi/boston-properties-wordpress-rest-openapi.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress logged-in cookie plus an X-WP-Nonce header. Advertised by the Access-Control-Allow-Headers\n    response header observed on https://www.bxp.com/wp-json/wp/v2/pages (2026-09-04).\n  sources:\n  - openapi/boston-properties-wordpress-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boston-properties/refs/heads/main/authentication/boston-properties-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Real-Estate
- Commercial Real Estate
- REIT
- Office Properties
- Workplace
- Fortune 1000
---
