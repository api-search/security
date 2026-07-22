---
api_key_in: []
auth_types:
- oauth2
- http
description: The Rachio Public API authenticates every request with an OAuth2 bearer token. The token is issued to a Rachio account and currently retrieved from the Rachio mobile app (Profile -> "Get API key"). There is no interactive authorization-code flow or documented scope surface; the single account token conveys full access to that account's people, devices, zones, schedules and webhooks.
kind: authentication
layout: security
method: searched
name: Rachio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rachio secures its APIs with oauth2 and http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rachio
provider_slug: rachio
scheme_count: 1
schemes:
- bearerFormat: OAuth2 token
  format: 'Authorization: Bearer <API_TOKEN>'
  header: Authorization
  location: header
  name: BearerToken
  scheme: bearer
  scopes: none-documented
  sources:
  - docs
  token_source: Retrieved from the Rachio mobile app (Profile icon -> API key -> Copy). One token per Rachio account.
  type: http
slug: rachio-authentication
source_filename: rachio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://rachio.readme.io/reference/authentication\ndocs: https://rachio.readme.io/reference/authentication\ndescription: >-\n  The Rachio Public API authenticates every request with an OAuth2 bearer token.\n  The token is issued to a Rachio account and currently retrieved from the Rachio\n  mobile app (Profile -> \"Get API key\"). There is no interactive authorization-code\n  flow or documented scope surface; the single account token conveys full access to\n  that account's people, devices, zones, schedules and webhooks.\nsummary:\n  types: [oauth2, http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    bearerFormat: OAuth2 token\n    location: header\n    header: Authorization\n    format: \"Authorization: Bearer <API_TOKEN>\"\n    token_source: >-\n      Retrieved from the Rachio mobile app (Profile icon -> API key -> Copy).\n      One\
  \ token per Rachio account.\n    scopes: none-documented\n    sources: [docs]\nnotes:\n  - No documented OAuth authorization/token endpoints; token is provisioned in-app.\n  - No documented scope model - the token is account-wide.\n  - Webhook callbacks are separately authenticated via an x-signature HMAC-SHA256 header keyed on the API token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rachio/refs/heads/main/authentication/rachio-authentication.yml
summary_line: oauth2/http · 1 scheme
tags:
- Company
- Smart Home
- IoT
- Irrigation
- Home Automation
- Water Management
- Webhooks
---
