---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Transcelestial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Transcelestial secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Transcelestial
provider_slug: transcelestial
scheme_count: 1
schemes:
- description: Token-based authentication over HTTPS for the CENTAURI device RESTful management API and Management UI. A per-device token authorizes viewing and modifying detailed configuration settings on the CENTAURI appliance.
  name: token
  scheme: bearer
  sources:
  - https://support.transcelestial.com/support/solutions/articles/51000334340-centauri-connectivity-requirements
  transport: https
  type: http
slug: transcelestial-authentication
source_filename: transcelestial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://support.transcelestial.com/support/solutions/articles/51000334340-centauri-connectivity-requirements\ndocs: https://support.transcelestial.com/support/solutions/articles/51000235505-centauri-product-manual\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    The CENTAURI Management API and Management UI are served on-device over HTTPS and require\n    authenticated access using token-based authentication. No OpenAPI/Swagger specification is\n    published, so this profile is derived from the CENTAURI support documentation rather than a\n    machine-readable security scheme.\nschemes:\n- name: token\n  type: http\n  scheme: bearer\n  transport: https\n  description: >-\n    Token-based authentication over HTTPS for the CENTAURI device RESTful management API and\n    Management UI. A per-device token authorizes viewing and modifying detailed configuration\n    settings on the CENTAURI\
  \ appliance.\n  sources:\n  - https://support.transcelestial.com/support/solutions/articles/51000334340-centauri-connectivity-requirements\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transcelestial/refs/heads/main/authentication/transcelestial-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Laser Communications
- Free-Space Optics
- Wireless
- Connectivity
- Backhaul
- Telecommunications
- Networking
- Satellite
- Device Management
---
