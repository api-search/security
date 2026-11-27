---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Epublys Authentication
name_suffix: Authentication
oauth_flows: []
overview: Epublys secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Epublys
provider_slug: epublys-com
scheme_count: 1
schemes:
- description: Optional API key (epl_xxx). Without it the free tier runs per IP address. Get a key (free) at https://epublys.com/account.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/epublys-com-openapi.json
  type: http
slug: epublys-com-authentication
source_filename: epublys-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/epublys-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Optional API key (epl_xxx). Without it the free tier runs per IP address. Get\n    a key (free) at https://epublys.com/account.\n  sources:\n  - openapi/epublys-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/epublys-com/authentication/epublys-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Tools
- EPUB
- Free
- Online
---
