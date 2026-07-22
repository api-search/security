---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nexon Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nexon Inc secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nexon Inc
provider_slug: nexon-inc
scheme_count: 1
schemes:
- description: Per-application API key. A developer signs in with a NEXON ID, registers an application, and is automatically issued an API key that acts as the authentication token. The key must be included in the x-nxopen-api-key HTTP header on every request to open.api.nexon.com. Usage limits are enforced per application.
  in: header
  issuance: https://openapi.nexon.com/my-application/create-app/
  name: nexonApiKey
  parameter_name: x-nxopen-api-key
  sources:
  - https://openapi.nexon.com/guide/request-api/
  type: apiKey
slug: nexon-inc-authentication
source_filename: nexon-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://openapi.nexon.com/guide/prepare-in-advance/\ndocs: https://openapi.nexon.com/guide/request-api/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: nexonApiKey\n  type: apiKey\n  in: header\n  parameter_name: x-nxopen-api-key\n  description: 'Per-application API key. A developer signs in with a NEXON ID, registers an\n    application, and is automatically issued an API key that acts as the authentication token.\n    The key must be included in the x-nxopen-api-key HTTP header on every request to\n    open.api.nexon.com. Usage limits are enforced per application.'\n  issuance: https://openapi.nexon.com/my-application/create-app/\n  sources:\n  - https://openapi.nexon.com/guide/request-api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexon-inc/refs/heads/main/authentication/nexon-inc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Gaming
- Video Games
- Game Data
- Developer API
- Open API
---
