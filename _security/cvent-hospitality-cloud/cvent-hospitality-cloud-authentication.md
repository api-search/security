---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cvent Hospitality Cloud Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cvent Hospitality Cloud secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cvent Hospitality Cloud
provider_slug: cvent-hospitality-cloud
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api-platform.cvent.com/reglink/v1/authentication/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/cvent-hospitality-cloud-openapi.yml
  type: oauth2
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/cvent-hospitality-cloud-openapi.yml
  type: http
slug: cvent-hospitality-cloud-authentication
source_filename: cvent-hospitality-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cvent-hospitality-cloud-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/reglink/v1/authentication/token\n    scopes: 2\n  sources:\n  - openapi/cvent-hospitality-cloud-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/cvent-hospitality-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/authentication/cvent-hospitality-cloud-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Catering
- Group Bookings
- Hospitality
- Hospitality Cloud
- Hotels
- Housing
- OAuth 2.0
- Passkey
- Reservations
- RFP
- Room Blocks
- Sales
- Sourcing
- Supplier Network
- Venues
---
