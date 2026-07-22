---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Roller Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: ROLLER secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: ROLLER
provider_slug: roller
scheme_count: 1
schemes:
- bearer_format: JWT
  flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - https://docs.roller.app/docs/api/authentication
  token_url: https://api.roller.app/token
  type: oauth2
slug: roller-authentication
source_filename: roller-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.roller.app/docs/api/authentication\ndocs: https://docs.roller.app/docs/api/authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  notes: >-\n    ROLLER APIs use an OAuth2 client-credentials flow. The consuming\n    application exchanges its client id and client secret (issued by ROLLER)\n    at the /token endpoint for a short-lived access token, which is then sent\n    as a Bearer token on API calls. Access tokens are short-lived; the expiry\n    is returned in the token response. Reuse the current token until a 401 is\n    received, then request a new one — requesting a new token per call can\n    trigger 429 rate-limit responses. API access is an add-on to a ROLLER\n    subscription; credentials are generated per venue via Getting API Access.\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://api.roller.app/token\n \
  \   bearer_format: JWT\n    sources: [https://docs.roller.app/docs/api/authentication]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roller/refs/heads/main/authentication/roller-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Venue Management
- Attractions
- Ticketing
- Bookings
- Point of Sale
- Payments
- Leisure
- Reservations
- Webhooks
---
