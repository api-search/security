---
api_key_in: []
api_specs:
- filename: vaynermedia-wordpress-content-openapi.json
  format: json
  label: VaynerMedia WordPress Content API
  slug: wordpress-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-wordpress-content-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vaynermedia Authentication
name_suffix: Authentication
oauth_flows: []
overview: VaynerMedia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VaynerMedia
provider_slug: vaynermedia
scheme_count: 1
schemes:
- description: WordPress Application Passwords. Advertised by the site's own route index (authentication.application-passwords.endpoints.authorization = https://vaynermedia.com/wp-admin/authorize-application.php). Required only for write operations and privileged reads; every operation in this document is callable anonymously.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/vaynermedia-wordpress-content-openapi.json
  type: http
slug: vaynermedia-authentication
source_filename: vaynermedia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/vaynermedia-wordpress-content-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords. Advertised by the site's own route index (authentication.application-passwords.endpoints.authorization\n    = https://vaynermedia.com/wp-admin/authorize-application.php). Required only for write operations\n    and privileged reads; every operation in this document is callable anonymously.\n  sources:\n  - openapi/vaynermedia-wordpress-content-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/authentication/vaynermedia-authentication.yml
summary_line: http · 1 scheme
tags:
- Advertising
- Agency
- Brand Strategy
- Content Production
- Creative
- Influencer Marketing
- Marketing
- Media Buying
- Social-Media
---
