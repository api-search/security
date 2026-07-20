---
api_key_in: []
auth_types:
- session
description: ''
kind: authentication
layout: security
method: searched
name: 1010Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: 1010data secures its APIs with session across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 1010data
provider_slug: 1010data
scheme_count: 1
schemes:
- description: Authentication to the Dynamic API is session-based. A client logs in with its usual Insights Platform credentials at the /api/!login endpoint (which can also be driven via the GUI), establishing a session. Subsequent calls operate against stateful QuickApp "environments" identified by a numeric tag returned from the /api/new endpoint. The XML API uses the same credential-based session model over HTTP.
  name: SessionLogin
  sources:
  - https://docs.1010data.com/DynamicAPI/DynamicAPI-Intro.html
  type: session
slug: 1010data-authentication
source_filename: 1010data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.1010data.com/DynamicAPI/DynamicAPI-Intro.html\ndocs: https://docs.1010data.com/DynamicAPI/DynamicAPI-Intro.html\nnote: >-\n  Derived from the 1010data Dynamic API and XML API documentation; no OpenAPI\n  securityScheme definition is published by the provider, so this profile is\n  captured from the auth documentation rather than mechanically from a spec.\nsummary:\n  types: [session]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: SessionLogin\n  type: session\n  description: >-\n    Authentication to the Dynamic API is session-based. A client logs in with\n    its usual Insights Platform credentials at the /api/!login endpoint (which\n    can also be driven via the GUI), establishing a session. Subsequent calls\n    operate against stateful QuickApp \"environments\" identified by a numeric tag\n    returned from the /api/new endpoint. The XML API uses the same\n    credential-based session model over\
  \ HTTP.\n  sources:\n  - https://docs.1010data.com/DynamicAPI/DynamicAPI-Intro.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1010data/refs/heads/main/authentication/1010data-authentication.yml
summary_line: session · 1 scheme
tags:
- Company
- Data Analytics
- Big Data
- Business Intelligence
- Cloud Analytics
- Data Management
- Retail Analytics
- Consumer Insights
- Capital Markets
- Data Sharing
---
