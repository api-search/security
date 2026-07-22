---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Nivelo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nivelo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nivelo
provider_slug: nivelo
scheme_count: 1
schemes:
- description: Nivelo's Scorer API is authenticated with a Bearer token (API key) passed in the HTTP Authorization header. A test environment / test API key is available for integration before going live.
  name: bearerAuth
  scheme: bearer
  sources:
  - https://nivelo.io/
  type: http
slug: nivelo-authentication
source_filename: nivelo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://nivelo.io/\ndocs: https://nivelo.io/\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Nivelo's Scorer API is authenticated with a Bearer token (API key) passed in the\n    HTTP Authorization header. A test environment / test API key is available for\n    integration before going live.\n  sources:\n  - https://nivelo.io/\nnotes: >-\n  Derived from Nivelo's published API description (RESTful Scorer endpoint at\n  https://api.nivelo.io/scorer using Bearer token authorization with an API key).\n  No OpenAPI is published by the provider, so this profile is captured from the docs\n  rather than derived from a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nivelo/refs/heads/main/authentication/nivelo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- ACH
- Fintech
- Payroll
- Risk
- Fraud Detection
- Money Movement
- Real-Time Payments
- Treasury
- FedNow
- RTP
---
