---
api_key_in:
- header
auth_types:
- clientCredentials
description: ''
kind: authentication
layout: security
method: searched
name: Local Logic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Local Logic secures its APIs with clientCredentials across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Local Logic
provider_slug: local-logic
scheme_count: 1
schemes:
- description: A client ID and secret pair, obtained by booking a demo, authorizes requests to the Local Logic API.
  in: header
  name: ClientCredentials
  sources:
  - https://docs.locallogic.co/
  type: apiKey
slug: local-logic-authentication
source_filename: local-logic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.locallogic.co/\ndocs: https://docs.locallogic.co/\nsummary:\n  types:\n  - clientCredentials\n  api_key_in:\n  - header\n  notes: >-\n    Local Logic API access requires a client ID and secret, issued after booking a\n    demo. Credentials are exchanged for/passed on API requests to the AWS-API-Gateway-fronted\n    host api.locallogic.co. No public OpenAPI specification is published, so scheme\n    details below are captured from the developer documentation rather than derived\n    from a spec.\nschemes:\n- name: ClientCredentials\n  type: apiKey\n  description: A client ID and secret pair, obtained by booking a demo, authorizes requests\n    to the Local Logic API.\n  in: header\n  sources:\n  - https://docs.locallogic.co/\nhost: https://api.locallogic.co\ngateway: aws-api-gateway\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/local-logic/refs/heads/main/authentication/local-logic-authentication.yml
summary_line: clientCredentials · 1 scheme
tags:
- Company
- Location Intelligence
- Real Estate
- Geospatial
- Neighborhoods
- Demographics
- Points of Interest
- Proptech
- Climate Risk
- Location Scores
---
