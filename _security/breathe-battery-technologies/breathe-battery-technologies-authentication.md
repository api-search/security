---
api_key_in: []
auth_types:
- bearer-token
description: ''
kind: authentication
layout: security
method: searched
name: Breathe Battery Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Breathe Battery Technologies secures its APIs with bearer-token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Breathe Battery Technologies
provider_slug: breathe-battery-technologies
scheme_count: 1
schemes:
- description: Token-based authentication handled by the SDK's login/refresh flow; token acquisition is not documented as a public endpoint.
  name: BearerToken
  scheme: bearer
  sources:
  - https://docs.breathebatteries.com/breathe-simulate-documentation/api_breathe_design_model/
  type: http
slug: breathe-battery-technologies-authentication
source_filename: breathe-battery-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.breathebatteries.com/breathe-simulate-documentation/api_breathe_design_model/\ndocs: https://docs.breathebatteries.com/\nsummary:\n  types:\n  - bearer-token\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Access is mediated by the first-party Python client (breathe-simulate / breathe-design). The\n    client authenticates against the Breathe cloud service using a token that it obtains and\n    refreshes automatically (an ensure_logged_in() step that \"checks if a valid token is\n    available and refreshes it if necessary\"). The service base URL is provisioned per account\n    via a BD_* environment variable and is not published in the public documentation. No public\n    OpenAPI specification, OAuth authorization/token endpoints, or API-key header scheme are\n    documented on the public surface.\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  sources:\n  - https://docs.breathebatteries.com/breathe-simulate-documentation/api_breathe_design_model/\n\
  \  description: >-\n    Token-based authentication handled by the SDK's login/refresh flow; token acquisition is not\n    documented as a public endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breathe-battery-technologies/refs/heads/main/authentication/breathe-battery-technologies-authentication.yml
summary_line: bearer-token · 1 scheme
tags:
- Company
- Battery
- Battery Simulation
- Electric Vehicles
- Energy Storage
- Cell Design
- Physics-Based Modeling
- Automotive
- Deep Tech
- Developer Tools
---
