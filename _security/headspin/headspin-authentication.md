---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Headspin Authentication
name_suffix: Authentication
oauth_flows: []
overview: HeadSpin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HeadSpin
provider_slug: headspin
scheme_count: 1
schemes:
- description: 'HeadSpin REST API calls authenticate with a HeadSpin API token passed as a Bearer token in the Authorization header (Authorization: Bearer <api_token>). Tokens are minted / retrieved via the Authentication API (POST https://api-dev.headspin.io/v0/api/token) and can be provisioned in the HeadSpin UI. The same token drives the `hs` CLI (hs auth init <token>) and the HeadSpin Appium load balancer endpoint (appium-dev.headspin.io:443/v0).'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://www.headspin.io/docs/auth-api
  type: http
slug: headspin-authentication
source_filename: headspin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.headspin.io/docs/auth-api\ndocs: https://www.headspin.io/docs/auth-api\nsummary:\n  types: [http]\n  http_scheme: bearer\n  token_model: api-token\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      HeadSpin REST API calls authenticate with a HeadSpin API token passed as a\n      Bearer token in the Authorization header (Authorization: Bearer <api_token>).\n      Tokens are minted / retrieved via the Authentication API\n      (POST https://api-dev.headspin.io/v0/api/token) and can be provisioned in the\n      HeadSpin UI. The same token drives the `hs` CLI (hs auth init <token>) and\n      the HeadSpin Appium load balancer endpoint (appium-dev.headspin.io:443/v0).\n    sources: [https://www.headspin.io/docs/auth-api]\nnotes: >-\n  No OpenAPI is published by HeadSpin; this profile is derived from the documented\n  Authentication API\
  \ guide. The API is key/token-based (no OAuth2 or OpenID Connect\n  scope surface), so scopes/ is not applicable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/headspin/refs/heads/main/authentication/headspin-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Testing
- Mobile
- Performance
- Real Device Testing
- Automation
- Appium
- OTT
- Quality Assurance
- Monitoring
---
