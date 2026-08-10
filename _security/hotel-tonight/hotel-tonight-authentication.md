---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hotel Tonight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hotel Tonight secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hotel Tonight
provider_slug: hotel-tonight
scheme_count: 1
schemes:
- applies_to: https://api-docs.hoteltonight.com/
  name: basicAuth
  scheme: basic
  sources:
  - https://api-docs.hoteltonight.com/
  type: http
slug: hotel-tonight-authentication
source_filename: hotel-tonight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api-docs.hoteltonight.com/\ndocs: https://api-docs.hoteltonight.com/\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  notes: >-\n    HotelTonight's partner/agent API is gated. The partner documentation portal\n    at api-docs.hoteltonight.com requires HTTP Basic authentication (username +\n    password) to view, and hotel partners sign in to the agent surface at\n    api.hoteltonight.com. No public OpenAPI securitySchemes are published, and\n    there is no open, self-service developer credentialing flow (no API keys,\n    OAuth 2.0, or OpenID Connect surfaced publicly).\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  applies_to: https://api-docs.hoteltonight.com/\n  sources: [https://api-docs.hoteltonight.com/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotel-tonight/refs/heads/main/authentication/hotel-tonight-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Travel
- Hotels
- Booking
- Hospitality
- Mobile
- Airbnb
---
