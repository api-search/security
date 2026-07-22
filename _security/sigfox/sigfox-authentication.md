---
api_key_in: []
api_specs:
- filename: doc.yaml
  format: yaml
  label: Sigfox Cloud API
  slug: sigfox-cloud-api
  spec_type: OpenAPI
  url: https://api.sigfox.com/v2/doc.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sigfox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sigfox secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sigfox
provider_slug: sigfox
scheme_count: 1
schemes:
- description: HTTP Basic authentication using the API access login (username) and password created in the Sigfox backend API access page. Authorization is governed by the profiles granted to the API access.
  name: basicAuth
  scheme: basic
  sources:
  - https://support.sigfox.com/docs/api-credential-creation
  type: http
slug: sigfox-authentication
source_filename: sigfox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://support.sigfox.com/docs/api-credential-creation\ndocs: https://support.sigfox.com/docs/api-credential-creation\nsummary:\n  types: [http]\n  scheme: basic\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    The Sigfox Cloud API authenticates with HTTP Basic credentials. An\n    \"API access\" is created in the Sigfox backend under a Group (Group tab >\n    API access > New). Each API access has a login (id) and password, plus a\n    display name, a timezone for responses, and one or more granted profiles\n    that define its role-based permissions. The credentials are sent as the\n    HTTP Basic Authorization header on every request. Rights are granted per\n    API access, so what endpoints an API user can call is determined by the\n    assigned profiles.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication using the API access login (username) and\n    password\
  \ created in the Sigfox backend API access page. Authorization is\n    governed by the profiles granted to the API access.\n  sources: [https://support.sigfox.com/docs/api-credential-creation]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sigfox/refs/heads/main/authentication/sigfox-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Industrial, Energy & Iot
- IoT
- LPWAN
- Connectivity
- Device Management
- Networking
- Telecommunications
---
