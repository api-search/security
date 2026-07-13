---
api_key_in: []
api_specs:
- filename: parkwhiz-openapi.yml
  format: yaml
  label: ParkWhiz Quotes & Locations API
  slug: parkwhiz-quotes-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/openapi/parkwhiz-openapi.yml
- filename: parkwhiz-openapi.yml
  format: yaml
  label: ParkWhiz Bookings API
  slug: parkwhiz-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/openapi/parkwhiz-openapi.yml
- filename: parkwhiz-openapi.yml
  format: yaml
  label: ParkWhiz Monthly Parking API
  slug: parkwhiz-monthly-parking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/openapi/parkwhiz-openapi.yml
- filename: parkwhiz-openapi.yml
  format: yaml
  label: ParkWhiz Venues & Events API
  slug: parkwhiz-venues-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/openapi/parkwhiz-openapi.yml
- filename: parkwhiz-openapi.yml
  format: yaml
  label: ParkWhiz Accounts & Vehicles API
  slug: parkwhiz-accounts-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/openapi/parkwhiz-openapi.yml
- filename: parkwhiz-openapi.yml
  format: yaml
  label: ParkWhiz Tickets API
  slug: parkwhiz-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/openapi/parkwhiz-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Parkwhiz Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: ParkWhiz secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: ParkWhiz
provider_slug: parkwhiz
scheme_count: 1
schemes:
- description: 'OAuth 2.0. Partner credentials (client_id, client_secret, redirect_uri) are issued by ParkWhiz to approved partners. Scopes: public (default), partner, mobile, internal, data.'
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://api.parkwhiz.com/v4/oauth/token
  - authorizationUrl: https://api.parkwhiz.com/v4/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.parkwhiz.com/v4/oauth/token
  name: oauth2
  sources:
  - openapi/parkwhiz-openapi.yml
  type: oauth2
slug: parkwhiz-authentication
source_filename: parkwhiz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parkwhiz-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.parkwhiz.com/v4/oauth/token\n    scopes: 3\n  - flow: authorizationCode\n    authorizationUrl: https://api.parkwhiz.com/v4/oauth/authorize\n    tokenUrl: https://api.parkwhiz.com/v4/oauth/token\n    scopes: 2\n  description: 'OAuth 2.0. Partner credentials (client_id, client_secret, redirect_uri) are\n    issued by ParkWhiz to approved partners. Scopes: public (default), partner, mobile, internal,\n    data.'\n  sources:\n  - openapi/parkwhiz-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/authentication/parkwhiz-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Parking
- Mobility
- Reservations
- Bookings
- Transportation
- Location
- Events
---
