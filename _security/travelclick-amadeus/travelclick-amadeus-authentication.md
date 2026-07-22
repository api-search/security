---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Travelclick Amadeus Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: TravelClick (Amadeus) secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: TravelClick (Amadeus)
provider_slug: travelclick-amadeus
scheme_count: 1
schemes:
- api_key_per_application: true
  flow: clientCredentials
  name: OAuth2
  non_production_key_contact: api-admin.tc@amadeus.com
  sources:
  - https://developer.travelclick.com/getstarted
  token_required_per_request: true
  type: oauth2
slug: travelclick-amadeus-authentication
source_filename: travelclick-amadeus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.travelclick.com/getstarted\ndocs: https://developer.travelclick.com/documentation\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  notes: >-\n    The Amadeus iHotelier BE (formerly TravelClick) REST APIs use the OAuth 2.0\n    authorization framework. An OAuth access token must be presented on every API\n    request. A unique API key is issued per application that an organization\n    registers on the developer portal; non-production API keys for interactive\n    testing are requested from api-admin.tc@amadeus.com. No public OpenAPI /\n    security scheme definition is available — the developer documentation is gated\n    behind portal registration — so this profile is captured from the published\n    Get Started guidance rather than derived from a spec.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flow: clientCredentials\n    token_required_per_request: true\n    api_key_per_application:\
  \ true\n    non_production_key_contact: api-admin.tc@amadeus.com\n    sources: [https://developer.travelclick.com/getstarted]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelclick-amadeus/refs/heads/main/authentication/travelclick-amadeus-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Ai Apps
- Hospitality
- Hotels
- Travel
- Booking Engine
- Reservations
- Distribution
- Central Reservation System
- OAuth2
---
