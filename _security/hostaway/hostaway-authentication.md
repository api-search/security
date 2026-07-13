---
api_key_in: []
api_specs:
- filename: hostaway-listings-api-openapi.yml
  format: yaml
  label: Hostaway Listings API
  slug: hostaway-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-listings-api-openapi.yml
- filename: hostaway-reservations-api-openapi.yml
  format: yaml
  label: Hostaway Reservations API
  slug: hostaway-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-reservations-api-openapi.yml
- filename: hostaway-calendar-api-openapi.yml
  format: yaml
  label: Hostaway Calendar API
  slug: hostaway-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-calendar-api-openapi.yml
- filename: hostaway-webhooks-api-openapi.yml
  format: yaml
  label: Hostaway Webhooks API
  slug: hostaway-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hostaway Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Hostaway secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Hostaway
provider_slug: hostaway
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.hostaway.com/v1/accessTokens
  name: OAuth2ClientCredentials
  sources:
  - openapi/hostaway-calendar-api-openapi.yml
  - openapi/hostaway-listings-api-openapi.yml
  - openapi/hostaway-reservations-api-openapi.yml
  - openapi/hostaway-webhooks-api-openapi.yml
  type: oauth2
slug: hostaway-authentication
source_filename: hostaway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hostaway-calendar-api-openapi.yml, openapi/hostaway-listings-api-openapi.yml,\n  openapi/hostaway-reservations-api-openapi.yml, openapi/hostaway-webhooks-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.hostaway.com/v1/accessTokens\n    scopes: 1\n  sources:\n  - openapi/hostaway-calendar-api-openapi.yml\n  - openapi/hostaway-listings-api-openapi.yml\n  - openapi/hostaway-reservations-api-openapi.yml\n  - openapi/hostaway-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/authentication/hostaway-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Vacation Rentals
- Short-Term Rentals
- Property Management
- Channel Manager
- Airbnb
- Vrbo
- Booking.com
- Expedia
- SaaS
---
