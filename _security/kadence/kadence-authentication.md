---
api_key_in: []
api_specs:
- filename: kadence-bookable-day-api-openapi.yml
  format: yaml
  label: Kadence Bookable Day API
  slug: kadence-bookable-day-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-bookable-day-api-openapi.yml
- filename: kadence-bookable-onsite-pass-api-openapi.yml
  format: yaml
  label: Kadence Bookable Onsite Pass API
  slug: kadence-bookable-onsite-pass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-bookable-onsite-pass-api-openapi.yml
- filename: kadence-bookable-space-api-openapi.yml
  format: yaml
  label: Kadence Bookable Space API
  slug: kadence-bookable-space-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-bookable-space-api-openapi.yml
- filename: kadence-booking-api-openapi.yml
  format: yaml
  label: Kadence Booking API
  slug: kadence-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-booking-api-openapi.yml
- filename: kadence-building-api-openapi.yml
  format: yaml
  label: Kadence Building API
  slug: kadence-building-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-building-api-openapi.yml
- filename: kadence-floor-api-openapi.yml
  format: yaml
  label: Kadence Floor API
  slug: kadence-floor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-floor-api-openapi.yml
- filename: kadence-neighborhood-api-openapi.yml
  format: yaml
  label: Kadence Neighborhood API
  slug: kadence-neighborhood-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-neighborhood-api-openapi.yml
- filename: kadence-space-api-openapi.yml
  format: yaml
  label: Kadence Space API
  slug: kadence-space-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-space-api-openapi.yml
- filename: kadence-user-api-openapi.yml
  format: yaml
  label: Kadence User API
  slug: kadence-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-user-api-openapi.yml
- filename: kadence-visit-api-openapi.yml
  format: yaml
  label: Kadence Visit API
  slug: kadence-visit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-visit-api-openapi.yml
- filename: kadence-visitor-api-openapi.yml
  format: yaml
  label: Kadence Visitor API
  slug: kadence-visitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-visitor-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Kadence Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Kadence secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Kadence
provider_slug: kadence
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials Grant
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.onkadence.co/oauth2/token
  name: oauth
  sources:
  - openapi/kadence-public-api-openapi.yml
  type: oauth2
slug: kadence-authentication
source_filename: kadence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/kadence-public-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.onkadence.co/oauth2/token\n    scopes: 1\n  description: OAuth 2.0 client credentials Grant\n  sources:\n  - openapi/kadence-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/authentication/kadence-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Workplace
- Hybrid Work
- Desk Booking
- Room Booking
- Space Management
- Visitor Management
- Workplace Analytics
- Facilities
- OAuth
---
