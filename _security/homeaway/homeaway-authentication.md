---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Homeaway Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: HomeAway * secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: HomeAway *
provider_slug: homeaway
scheme_count: 1
schemes:
- credentials:
  - client_id
  - client_secret
  flows:
  - description: Two-legged client authentication for public API access.
    flow: clientCredentials
  - description: Three-legged flow to access an end user's personal HomeAway data.
    flow: authorizationCode
  name: OAuth2
  registration: https://www.homeaway.com/platform/myClients
  sources:
  - github.com/homeaway/homeaway_api_ruby
  type: oauth2
slug: homeaway-authentication
source_filename: homeaway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/homeaway/homeaway_api_ruby\ndocs: https://www.homeaway.com/platform/myClients\nnote: >-\n  No OpenAPI is available for HomeAway (brand retired into Expedia Group / Vrbo),\n  so this profile is derived from the first-party Ruby SDK documentation rather\n  than a machine-readable spec. The HomeAway API used OAuth 2.0: applications\n  register for a client id and client secret at the developer platform, then use\n  either two-legged (client-credentials) access for public data or a three-legged\n  authorization-code flow to access a user's personal HomeAway data.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials, authorizationCode]\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    description: Two-legged client authentication for public API access.\n  - flow: authorizationCode\n    description: Three-legged flow to access an end user's personal HomeAway data.\n\
  \  credentials:\n  - client_id\n  - client_secret\n  registration: https://www.homeaway.com/platform/myClients\n  sources: [github.com/homeaway/homeaway_api_ruby]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homeaway/refs/heads/main/authentication/homeaway-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Consumer
- Vacation Rentals
- Travel
- Hospitality
- Marketplace
- Bookings
- Property Management
---
