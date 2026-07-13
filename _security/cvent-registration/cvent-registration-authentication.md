---
api_key_in: []
api_specs:
- filename: cvent-registration-openapi.yml
  format: yaml
  label: Cvent Registration REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cvent Registration Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cvent Registration secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cvent Registration
provider_slug: cvent-registration
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 9
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/cvent-registration-openapi.yml
  type: oauth2
- description: Client ID / client secret Basic auth used only for the /ea/oauth2/token call.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/cvent-registration-openapi.yml
  type: http
slug: cvent-registration-authentication
source_filename: cvent-registration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cvent-registration-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n    scopes: 9\n  sources:\n  - openapi/cvent-registration-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Client ID / client secret Basic auth used only for the /ea/oauth2/token call.\n  sources:\n  - openapi/cvent-registration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/authentication/cvent-registration-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Attendee Management
- Attendees
- Conferences
- Event Management
- Events
- OAuth 2.0
- On-Site Check-In
- Payments
- Registration
- REST API
- Ticketing
- Webhooks
---
