---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Staffbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Staffbase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Staffbase
provider_slug: staffbase
scheme_count: 1
schemes:
- description: API access uses HTTP Basic authentication carrying a Staffbase API token. Tokens are generated per-installation in the Staffbase Studio admin and scope access to a branch/space. Unauthenticated calls return HTTP 401 with a JSON error envelope (ref ERROR_LOGIN_REQUIRED).
  evidence:
  - 'GET https://app.staffbase.com/api/users -> 401 application/json {ref: ERROR_LOGIN_REQUIRED}'
  name: apiToken
  scheme: basic
  type: http
slug: staffbase-authentication
source_filename: staffbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.staffbase.com/api/\ndocs: https://developers.staffbase.com/api/\nnotes: >-\n  Derived from the Staffbase developer portal and a live 401 challenge against the\n  API base. No downloadable OpenAPI/Swagger definition is published, so this profile\n  is documented from the developer portal rather than mechanically derived from a spec.\nbase_url: https://app.staffbase.com/api\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: apiToken\n    type: http\n    scheme: basic\n    description: >-\n      API access uses HTTP Basic authentication carrying a Staffbase API token.\n      Tokens are generated per-installation in the Staffbase Studio admin and scope\n      access to a branch/space. Unauthenticated calls return HTTP 401 with a JSON\n      error envelope (ref ERROR_LOGIN_REQUIRED).\n    evidence:\n      - \"GET https://app.staffbase.com/api/users ->\
  \ 401 application/json {ref: ERROR_LOGIN_REQUIRED}\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/staffbase/refs/heads/main/authentication/staffbase-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Employee Communications
- Internal Communications
- Employee Experience
- Intranet
- Employee App
- Email
- HR Tech
- Enterprise
---
