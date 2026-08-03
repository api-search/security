---
api_key_in:
- header
api_specs:
- filename: abcuro-content-openapi.yml
  format: yaml
  label: Abcuro Content API (WordPress REST)
  slug: abcuro-content-api-wordpress-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-content-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Abcuro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Abcuro secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Abcuro
provider_slug: abcuro
scheme_count: 2
schemes:
- description: WordPress application passwords (RFC 7617 Basic over TLS). The live route index advertises the authorization endpoint at https://abcuro.com/wp-admin/authorize-application.php. Required for every write operation and for the edit context; not available to the public.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/abcuro-content-openapi.yml
  type: http
- description: WordPress cookie authentication paired with an X-WP-Nonce header; used by the site's own admin and block-editor UI.
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/abcuro-content-openapi.yml
  type: apiKey
slug: abcuro-authentication
source_filename: abcuro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/abcuro-content-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application passwords (RFC 7617 Basic over TLS). The live route index\n    advertises the authorization endpoint at https://abcuro.com/wp-admin/authorize-application.php.\n    Required for every write operation and for the edit context; not available to the public.\n  sources:\n  - openapi/abcuro-content-openapi.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress cookie authentication paired with an X-WP-Nonce header; used by the\n    site's own admin and block-editor UI.\n  sources:\n  - openapi/abcuro-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/authentication/abcuro-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- biotechnology
- pharmaceuticals
- immunology
- autoimmune-disease
- oncology
- clinical-trials
- life-sciences
- drug-development
- healthcare
- content-api
- wordpress
---
