---
api_key_in: []
auth_types: []
description: Authentication profile for the Purchaser sourcing API, captured from the public API & Integrations overview. Full authentication guides are available to Purchaser customers behind login.
kind: authentication
layout: security
method: searched
name: Purchaser Authentication
name_suffix: Authentication
oauth_flows: []
overview: Purchaser declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Purchaser
provider_slug: purchaser
scheme_count: 2
schemes:
- description: API-key based authentication. Keys carry team and environment scoping and can be rotated without downtime.
  id: api_key
  in: header
  rotation: supported
  scoping:
  - team
  - environment
  type: apiKey
- applies_to: application-ui
  description: Single sign-on (SSO) with role-based access control governs the Purchaser application; used for human access rather than programmatic API calls.
  id: sso
  type: openIdConnect
slug: purchaser-authentication
source_filename: purchaser-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://purchaser.ai/api-and-integrations (public API & Integrations overview)\ndocs: https://docs.purchaser.ai\nname: Purchaser API Authentication\ndescription: >-\n  Authentication profile for the Purchaser sourcing API, captured from the\n  public API & Integrations overview. Full authentication guides are available\n  to Purchaser customers behind login.\nschemes:\n  - id: api_key\n    type: apiKey\n    in: header\n    description: >-\n      API-key based authentication. Keys carry team and environment scoping and\n      can be rotated without downtime.\n    rotation: supported\n    scoping:\n      - team\n      - environment\n  - id: sso\n    type: openIdConnect\n    description: >-\n      Single sign-on (SSO) with role-based access control governs the Purchaser\n      application; used for human access rather than programmatic API calls.\n    applies_to: application-ui\nnotes: >-\n  OAuth2 scopes are not documented on\
  \ the public overview. Programmatic access\n  uses API keys; SSO/RBAC secures the web application.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/purchaser/refs/heads/main/authentication/purchaser-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Ai
- Procurement
- Sourcing
- RFQ
- Supply Chain
- Construction
- Enterprise
---
