---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Burner Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Burner secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Burner
provider_slug: burner
scheme_count: 1
schemes:
- evidence: 'llms.txt: "OAuth 2.0 authentication for API access and third-party integrations"; BASK README "Request Burner OAuth app credentials"; BurnerApi.js sends `Authorization: Bearer ${this.token}`.'
  flows:
  - flow: authorizationCode
  format: Bearer <access_token>
  header: Authorization
  name: OAuth2
  sources:
  - https://www.burnerapp.com/llms.txt
  - https://github.com/adhoclabs/burner-app-starter-kit
  token_transport: bearer
  type: oauth2
slug: burner-authentication
source_filename: burner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://www.burnerapp.com/llms.txt ;\n  https://github.com/adhoclabs/burner-app-starter-kit (src/core/BurnerApi.js, README Authentication section)\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  token_transport: bearer\nnotes: >-\n  Burner authenticates API access with OAuth 2.0. Third-party apps request Burner\n  OAuth app credentials, obtain an access token, and call the API with an\n  `Authorization: Bearer <token>` header. The official client also sends an\n  `X-Application-Version` header. Derived from the documented developer surface\n  (llms.txt) and the first-party Burner App Starter Kit client, which is the\n  authoritative reference for the live request shape. No published OpenAPI spec.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n    token_transport: bearer\n    header: Authorization\n    format: \"Bearer <access_token>\"\n\
  \    sources:\n      - https://www.burnerapp.com/llms.txt\n      - https://github.com/adhoclabs/burner-app-starter-kit\n    evidence: >-\n      llms.txt: \"OAuth 2.0 authentication for API access and third-party\n      integrations\"; BASK README \"Request Burner OAuth app credentials\";\n      BurnerApi.js sends `Authorization: Bearer ${this.token}`.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/burner/refs/heads/main/authentication/burner-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Phone Numbers
- SMS
- MMS
- Voice
- Messaging
- Telephony
- Privacy
- Communications
- Second Phone Number
- OAuth
- Webhooks
---
