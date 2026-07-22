---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Rimsys Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rimsys secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rimsys
provider_slug: rimsys
scheme_count: 1
schemes:
- bearerFormat: access_token
  description: 'Bearer access token passed in the Authorization header, per the Rimsys developer portal code samples (Authorization: Bearer ${accessToken}).'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.rimsys.io/
  type: http
slug: rimsys-authentication
source_filename: rimsys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.rimsys.io/\ndocs: https://docs.rimsys.io/\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    The Rimsys developer portal (Theneo-hosted) documents API requests authenticated with a\n    bearer access token supplied in the HTTP Authorization header (Authorization: Bearer\n    <accessToken>). No public OpenAPI specification was available for mechanical derivation;\n    this profile is captured from the published documentation and code samples.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: access_token\n  description: 'Bearer access token passed in the Authorization header, per the Rimsys developer\n    portal code samples (Authorization: Bearer ${accessToken}).'\n  sources:\n  - https://docs.rimsys.io/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rimsys/refs/heads/main/authentication/rimsys-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Vertical Software
- Regulatory
- Medical Devices
- MedTech
- Regulatory Information Management
- UDI
- Compliance
- Life Sciences
---
